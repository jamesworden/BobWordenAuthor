<script>
  import ProfileCard from './ProfileCard.svelte';
  import TriangleGraphic from './TriangleGraphic.svelte';
  import MessageForm from './MessageForm.svelte';

  function readMore() {
    const element = document.getElementById('read-more');
    if (element) {
      element.scrollIntoView({ behavior: 'smooth' });
    }
  }
</script>

<svelte:head>
  <title>Home</title>
  <meta
    name="description"
    content="Bob Worden's Latest Title, How to Stop Wars and Save the World"
  />
</svelte:head>

<section class="flex page-content-width md:mx-auto w-full">
  <div class="hidden md:block pl-4 mb-8">
    <ProfileCard />
  </div>

  <section class="diagonal-bg py-8 pr-8 md:pl-8 flex flex-1">
    <div class="py-16 bg-gray-50 flex flex-col justify-between flex-1">
      <div class="px-4">
        <div class="mb-12">
          <h3 class="uppercase text-gray-600 tracking-widest mb-4">
            Bob Worden's New Title
          </h3>

          <h1
            class="font-semibold text-gray-700 mb-4 text-4xl sm:text-5xl md:text-6xl"
          >
            How to Stop Wars <br />and Save the World
          </h1>

          <h2>Lessons in Negotiation, Settlement, <br />and Leadership</h2>
        </div>

        <button
          class="text-white bg-yellow-600 py-2 px-8 uppercase tracking-wide shadow-lg font-bold hover:scale-105 hover:bg-yellow-500 transition"
          on:click={readMore}>Read More</button
        >
      </div>

      <div class="flex justify-end md:pr-16">
        <TriangleGraphic />
      </div>
    </div>
  </section>
</section>

<section id="read-more" class="bg-slate-800 py-12 md:p-12">
  <div
    class="page-content-width mx-auto grid grid-cols-1 md:grid-cols-3 gap-4 text-white"
  >
    <div class="px-4">
      <h2 class="font-semibold mb-4 max-w-xl">
        Soon to be available on Amazon and booksellers everywhere.
      </h2>
      <hr class="h-px w-1/6 bg-white" />
    </div>

    <div class="px-4 max-w-xl">
      Soon to be available on Amazon and booksellers everywhere. In this new
      short book, How to Stop Wars and Save the World, Bob Worden analyzes the
      conflicts which led to fighting three American wars. He reveals surprising
      stories which most people don’t know. Learn how to settle disputes of any
      kind, while learning the key facts and circumstances which ignited the
      Revolutionary, Civil and Vietnam wars. Using the mistakes leaders made in
      these conflicts,
    </div>

    <div class="px-4 max-w-xl">
      Bob explains principles of settlement and negotiation, and demonstrates
      why settlement, if possible, is always preferable to going to war. Bob
      avoids unnecessary details and dates, and tells the stories behind the
      wars, captivating readers, who are fascinated to learn what these wars
      were all about, and why we need to settle, rather than fight, whenever
      possible.
    </div>
  </div>
</section>

<section class="py-12 md:p-12">
  <div class="page-content-width mx-auto grid grid-cols-1 md:grid-cols-3 gap-4">
    <div class="px-4">
      <h2 class="font-semibold mb-4 max-w-xl">
        Mediation resolves conflict fast.
      </h2>
      <hr class="h-px w-1/6 bg-black" />
    </div>

    <div class="px-4 max-w-xl">
      Mediation is when a neutral person with special knowledge seeks to resolve
      a lawsuit or other dispute, by meeting with the parties to the lawsuit in
      order to obtain a swift and fair negotiated settlement. Arbitration
      decides disputes with informal hearings before one arbitrator or several
      arbitrators.
    </div>

    <div class="px-4 max-w-xl">
      There is no jury. Arbitration is much quicker and much less expensive that
      going to trial before a Court. Unlike mediation, arbitration has no
      negotiation. The arbitrator hears the evidence in a case and decides if
      there will be any award and, if so, how much the award will be.
    </div>
  </div>
</section>

<section class=" px-4">
  <div
    class="page-content-width mx-auto flex flex-col md:flex-row text-white shadow-xl"
  >
    <div class="flex-1 bg-yellow-600 p-4 py-12 md:px-12">
      <h2 class="font-semibold text-3xl mb-4">Experience</h2>

      <p class="mb-4 max-w-xl">
        Mediator, Arbitrator and Settlement Counsel with track record of early
        resolution of lawsuits, handling major cases throughout New York State.
        Extensive experience in high exposure, large-loss and catastrophic
        general liability, premises, motor vehicle and property damages claims.
        Areas of special interest include medical malpractice, products
        liability and construction accidents under New York’s Labor Law.
      </p>

      <a href="/about" class="no-underline italic">Learn More →</a>
    </div>

    <div class="flex-1 flex flex-col">
      <div
        class="flex-1 bg-slate-700 transition pl-4 md:pl-16 flex flex-col justify-around group hover:bg-yellow-600 py-4"
      >
        <div class="flex">
          <div class="h-20 border-l border-gray-300 mr-4"></div>
          <div class="flex flex-col justify-around">
            <ul class="list-none flex flex-col">
              <h2 class="font-semibold">National Mediation and Arbitration</h2>
              <li
                class="group-hover:scale-110 group-hover:translate-x-6 transition"
              >
                <a
                  href="https://www.namadr.com/neutrals-bio/bob-worden-esq/"
                  target="_blank"
                  class="no-underline transition italic">Mediator →</a
                >
              </li>
              <li
                class="group-hover:scale-110 group-hover:translate-x-6 transition"
              >
                <a
                  href="https://www.namadr.com/neutrals-bio/bob-worden-esq/"
                  target="_blank"
                  class="no-underline transition italic">Lecturer →</a
                >
              </li>
            </ul>
          </div>
        </div>
      </div>

      <a
        href="https://www.lwrlawyer.com/attorney/robert-p-worden-jr/"
        target="_blank"
        class="flex-1 bg-slate-600 hover:bg-yellow-600 transition pl-4 md:pl-16 flex flex-col justify-around py-4"
      >
        <div class="flex">
          <div class="h-20 border-l border-gray-300 mr-4"></div>
          <div class="flex flex-col justify-around">
            <ul class="list-none flex flex-col">
              <h2 class="font-semibold">Law Firm</h2>
              <h3>Lawrence Worden Rainis & Bard P.C.</h3>
              <li class="italic">Learn More →</li>
            </ul>
          </div>
        </div>
      </a>

      <a
        href="https://www.jdsupra.com/legalnews/is-mediation-conducted-through-36050/"
        target="_blank"
        class="flex-1 bg-slate-500 hover:bg-yellow-600 transition pl-4 md:pl-16 flex flex-col justify-around py-4"
      >
        <div class="flex">
          <div class="h-20 border-l border-gray-300 mr-4"></div>
          <div class="flex flex-col justify-around">
            <ul class="list-none flex flex-col">
              <h2 class="font-semibold">Articles</h2>
              <li class="italic">Learn More →</li>
            </ul>
          </div>
        </div>
      </a>
    </div>
  </div>
</section>

<section class="page-content-width mx-auto flex w-full">
  <div class="diagonal-bg p-8 flex flex-1">
    <div class="h-96 py-16 pl-0 bg-gray-50 flex flex-1 justify-between">
      <div></div>
      <div
        class="flex flex-col justify-between absolute z-10 bg-gray-50 bg-opacity-80 -mt-4"
      >
        <MessageForm />
      </div>
      <div class="flex flex-col justify-end md:pr-8">
        <TriangleGraphic />
      </div>
    </div>
  </div>
</section>

<style>
  .diagonal-bg {
    background-color: transparent;
    background-image: -webkit-linear-gradient(
      -50deg,
      transparent 75%,
      #e5e7eb 25%
    );
  }
</style>
