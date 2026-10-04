<script>
  import TriangleGraphic from './TriangleGraphic.svelte';
</script>

<svelte:head>
  <title>Bob Worden - Mediator, Arbitrator & Author</title>
  <meta
    name="description"
    content="Bob Worden - Mediator, Arbitrator, Settlement Counsel and Author of How to Stop Wars and Save the World"
  />
</svelte:head>

<!-- Hero Section -->
<section class="flex bw-page-content-width md:mx-auto w-full">
  <section class="bw-diagonal-bg py-8 pr-8 md:pl-8 flex flex-1">
    <div class="py-16 bg-gray-50 flex flex-col justify-between flex-1 px-4 md:px-8">
      <div class="px-4 max-w-4xl">
        <h3 class="uppercase text-gray-600 tracking-widest mb-4">
          <span>Welcome</span>
        </h3>

        <h1 class="font-semibold text-gray-700 text-4xl sm:text-5xl md:text-6xl mb-6">
          Bob Worden, Esq.
        </h1>

        <h2 class="text-2xl md:text-3xl text-gray-600 mb-8">
          Mediator, Arbitrator, Settlement Counsel & Author
        </h2>

        <p class="text-lg text-gray-700 mb-8 max-w-2xl">
          Experienced legal professional specializing in mediation, arbitration, and dispute resolution throughout New York State.
          Author of insightful commentaries on American history and politics.
        </p>

        <div class="flex gap-4">
          <a
            href="/book"
            class="text-white bg-yellow-600 py-3 px-8 uppercase tracking-wide shadow-lg font-bold hover:scale-105 hover:bg-yellow-500 transition">
            View Book
          </a>
          <a
            href="/about"
            class="text-gray-700 bg-white border-2 border-gray-700 py-3 px-8 uppercase tracking-wide shadow-lg font-bold hover:scale-105 hover:bg-gray-100 transition">
            About Bob
          </a>
        </div>
      </div>

      <div class="justify-end md:pr-16 hidden md:flex">
        <TriangleGraphic />
      </div>
    </div>
  </section>
</section>

<!-- Latest Commentaries Section -->
<section class="bg-white py-12 md:p-12">
  <div class="bw-page-content-width mx-auto px-4">
    <h2 class="font-semibold text-3xl md:text-4xl mb-8 text-gray-800">Latest Commentaries</h2>

    <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
      <!-- Article 1 -->
      <a href="/articles/futility-of-violence" class="group block bg-gray-50 shadow-lg hover:shadow-xl transition-all p-6 border-l-4 border-yellow-600">
        <h3 class="font-semibold text-xl md:text-2xl text-gray-800 mb-3 group-hover:text-yellow-600 transition">
          The Futility of Violence in the Quest for Change
        </h3>
        <p class="text-gray-600 text-sm mb-4">October 2, 2026</p>
        <p class="text-gray-700 mb-4">
          Examining historical political violence in America and the power of voting as the true path to change.
          A look back at 150 years of American political conflict and what it teaches us today.
        </p>
        <span class="text-yellow-600 font-semibold group-hover:underline">Read More →</span>
      </a>

      <!-- Article 2 -->
      <a href="/articles/french-revolution" class="group block bg-gray-50 shadow-lg hover:shadow-xl transition-all p-6 border-l-4 border-yellow-600">
        <h3 class="font-semibold text-xl md:text-2xl text-gray-800 mb-3 group-hover:text-yellow-600 transition">
          Progressive Mistakes of the French Revolution
        </h3>
        <p class="text-gray-600 text-sm mb-4">April 20, 2026</p>
        <p class="text-gray-700 mb-4">
          Exploring the French Revolution's impractical reforms and drawing parallels to modern American politics.
          Why capable leadership matters more than ideology.
        </p>
        <span class="text-yellow-600 font-semibold group-hover:underline">Read More →</span>
      </a>
    </div>
  </div>
</section>

<!-- Mediation Section -->
<section class="py-12 md:p-12 bg-gray-50">
  <div class="bw-page-content-width mx-auto grid grid-cols-1 md:grid-cols-3 gap-4">
    <div class="px-4">
      <h2 class="font-semibold mb-4 max-w-xl text-2xl md:text-3xl">
        Mediation resolves conflict fast.
      </h2>
      <hr class="h-px w-1/6 bg-black" />
    </div>

    <div class="px-4 max-w-xl">
      Mediation is when a neutral person with special knowledge seeks to resolve
      a lawsuit or other dispute, by meeting with the parties in order to obtain
      a swift and fair negotiated settlement. Arbitration decides disputes with
      informal hearings before one arbitrator or several arbitrators.
    </div>

    <div class="px-4 max-w-xl">
      There is no jury. Arbitration is much quicker and much less expensive that
      going to trial before a Court. Unlike mediation, arbitration has no
      negotiation. The arbitrator hears the evidence in a case and decides if
      there will be any award and, if so, how much the award will be.
    </div>
  </div>
</section>

<!-- Experience Section -->
<section class="pb-16 px-4">
  <div class="bw-page-content-width mx-auto flex flex-col md:flex-row text-white shadow-xl">
    <div class="flex-1 bg-yellow-600 p-4 py-12 md:px-12">
      <h2 class="font-semibold text-3xl mb-4">Experience</h2>

      <p class="mb-4 max-w-xl">
        Mediator, Arbitrator and Settlement Counsel with track record of early
        resolution of lawsuits, handling major cases throughout New York State.
        Extensive experience in high exposure, large-loss and catastrophic
        general liability, premises, motor vehicle and property damages claims.
        Areas of special interest include medical malpractice, products
        liability and construction accidents under New York's Labor Law.
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
                  href="https://profiles.superlawyers.com/new-york/melville/lawyer/robert-p-worden/2002b209-2407-432d-b0bd-5eec0cc0383f.html"
                  target="_blank"
                  class="no-underline transition italic">Lecturer →</a
                >
              </li>
            </ul>
          </div>
        </div>
      </div>

      <a
        href="https://pvrklaw.com/attorney/robert-worden/"
        target="_blank"
        class="flex-1 bg-slate-600 hover:bg-yellow-600 transition pl-4 md:pl-16 flex flex-col justify-around py-4"
      >
        <div class="flex">
          <div class="h-20 border-l border-gray-300 mr-4"></div>
          <div class="flex flex-col justify-around">
            <ul class="list-none flex flex-col">
              <h2 class="font-semibold">Law Firm</h2>
              <h3>Perry, Van Etten, Rainis & Kutner, LLP</h3>
              <li class="italic">Learn More →</li>
            </ul>
          </div>
        </div>
      </a>

      <a
        href="https://www.jdsupra.com/authors/bob-worden/"
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
