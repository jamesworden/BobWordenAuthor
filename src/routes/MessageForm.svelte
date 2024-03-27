<script lang="ts">
  enum FormStatus {
    NotSent,
    Sending,
    Sent,
    Errored
  }

  let formStatus = FormStatus.NotSent;
  let name = '';
  let email = '';
  let message = '';
  let hasSentMessage = false;

  const handleInput = () => {
    const textarea = document.getElementById('message');
    textarea!.style.height = 'auto'; // Reset height to auto to calculate new height
    textarea!.style.height = textarea!.scrollHeight + 'px'; // Set height to the calculated scrollHeight
  };

  const handleSubmit = () => {
    if (!name || !email || !message) {
      alert('Please fill in all fields');
      return;
    }

    if (!isValidEmail(email)) {
      alert('Please enter a valid email address');
      return;
    }

    console.log('Name:', name);
    console.log('Email:', email);
    console.log('Message:', message);

    formStatus = FormStatus.Sending;

    fetch('https://act4822wla.execute-api.us-east-1.amazonaws.com/Production', {
      method: 'POST',
      mode: 'cors',
      cache: 'no-cache',
      body: JSON.stringify({
        name,
        email,
        message
      }),
      headers: {
        'Content-type': 'application/json; charset=UTF-8'
      }
    })
      .then((x) => {
        if (x.status === 200) {
          hasSentMessage = true;
          formStatus = FormStatus.Sent;
          name = '';
          email = '';
          message = '';
        } else {
          throw new Error('Failed to send message.');
        }
      })
      .catch(() => {
        formStatus = FormStatus.Errored;
      });
  };

  const isValidEmail = (email: string) => {
    const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
    return emailRegex.test(email);
  };
</script>

<section>
  <h1 class="text-3xl mb-6 text-slate-800 font-semibold">
    {#if formStatus === FormStatus.Errored}
      <p>Oops, something went wrong!</p>
    {:else if formStatus === FormStatus.NotSent}
      <p>Reach out to Bob.</p>
    {:else if formStatus === FormStatus.Sending}
      <p>Sending...</p>
    {:else if formStatus === FormStatus.Sent}
      <p>Message sent!</p>
    {/if}
  </h1>

  <form
    on:submit|preventDefault={handleSubmit}
    class="w-80 flex flex-col gap-y-8"
  >
    <label class="flex">
      <span class="mr-2">Name:</span>
      <input
        type="text"
        bind:value={name}
        required
        maxlength="128"
        class="w-full bg-transparent outline-none border-black border-b"
      />
    </label>
    <label class="flex">
      <span class="mr-2">Email:</span>
      <input
        type="email"
        bind:value={email}
        required
        maxlength="128"
        class="w-full bg-transparent outline-none border-black border-b"
      />
    </label>
    <label class="flex">
      <span class="mr-2">Message:</span>
      <textarea
        bind:value={message}
        required
        on:input={handleInput}
        style="resize: none; overflow-y: hidden;"
        rows="1"
        id="message"
        maxlength="512"
        class="w-full bg-transparent outline-none border-black border-b"
      ></textarea>
    </label>

    <div>
      <button
        type="submit"
        class="text-white bg-yellow-600 py-2 px-16 uppercase tracking-wide shadow-lg font-bold hover:scale-105 hover:bg-yellow-500 transition mt-2"
        on:click={() => {}}
      >
        {#if hasSentMessage}
          <p>Send Another</p>
        {:else}
          <p>Send</p>
        {/if}
      </button>
    </div>
  </form>
</section>

<style>
  input:-webkit-autofill,
  input:-webkit-autofill:hover,
  input:-webkit-autofill:focus,
  input:-webkit-autofill:active {
    -webkit-background-clip: text;
    transition: background-color 5000s ease-in-out 0s;
    box-shadow: inset 0 0 20px 20px transparent;
  }
</style>
