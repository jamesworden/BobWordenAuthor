<script>
  import book_cover from '$lib/images/book-cover.jpg';
</script>

<svelte:head>
  <title>Bob's Book - How to Stop Wars and Save the World</title>
  <meta
    name="description"
    content="Bob Worden's Latest Title, How to Stop Wars and Save the World"
  />
</svelte:head>

<div class="bw-page-content-width mx-auto py-12 px-4">
  <!-- Book Header Section -->
  <section class="mb-12">
    <div class="flex flex-col md:flex-row gap-8 items-start">
      <!-- Book Cover -->
      <div class="flex-shrink-0">
        <div class="bg-slate-600 p-3 shadow-lg max-w-xs">
          <picture>
            <img
              src={book_cover}
              alt="How to Stop Wars and Save the World"
              class="w-full -mt-6 -ml-6"
            />
          </picture>
        </div>
      </div>

      <!-- Book Info -->
      <div class="flex-1">
        <h3 class="uppercase text-gray-600 tracking-widest mb-2 text-sm">
          <span>Bob Worden's New Title</span>
        </h3>

        <h1 class="font-semibold text-gray-700 text-3xl md:text-4xl mb-3">
          How to Stop Wars and Save the World
        </h1>

        <h2 class="text-xl text-gray-600 mb-6">
          Lessons in Negotiation, Settlement, and Leadership
        </h2>

        <p class="text-gray-600 mb-6">Copyright © 2024</p>

        <a
          href="https://a.co/d/ejuS2hT"
          class="inline-block text-white bg-yellow-600 py-3 px-8 uppercase tracking-wide shadow-lg font-bold hover:scale-105 hover:bg-yellow-500 transition"
          target="_blank">
          Order Now
        </a>
      </div>
    </div>
  </section>

  <!-- Now Available on Amazon Section -->
  <section id="read-more" class="bg-slate-800 py-12 px-8 md:p-12 mb-12">
    <div class="grid grid-cols-1 md:grid-cols-3 gap-6 text-white">
      <div>
        <h2 class="font-semibold mb-4 text-2xl">
          <a href="https://a.co/d/ejuS2hT" class="hover:text-yellow-500 transition">Now available on Amazon.</a>
        </h2>
        <hr class="h-px w-1/6 bg-white" />
      </div>

      <div class="max-w-xl">
        In this new book, <a class="underline hover:text-yellow-500 transition" href="https://a.co/d/ejuS2hT">How to Stop Wars and Save the World</a>, Bob Worden analyzes
        the conflicts which led to fighting three American wars. He reveals
        surprising stories which most people don't know. Learn how to settle
        disputes of any kind, while learning the key facts and circumstances which
        ignited the Revolutionary, Civil and Vietnam wars. Using the mistakes
        leaders made in these conflicts,
      </div>

      <div class="max-w-xl">
        Bob explains principles of settlement and negotiation, and demonstrates
        why settlement, if possible, is always preferable to going to war. Bob
        avoids unnecessary details and dates, and tells the stories behind the
        wars, captivating readers, who are fascinated to learn what these wars
        were all about, and why we need to settle, rather than fight, whenever
        possible.
      </div>
    </div>
  </section>

</div>
