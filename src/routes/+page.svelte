<script>
  import ProfileCard from './ProfileCard.svelte';
  import TriangleGraphic from './TriangleGraphic.svelte';

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

<section class="flex page-content-width px-2 mx-auto">
  <div>
    <ProfileCard />
  </div>

  <section class="diagonal-bg p-8 flex flex-1">
    <div class="p-16 bg-gray-50 flex flex-col justify-between flex-1">
      <div>
        <div class="mb-12">
          <h3 class="uppercase text-gray-600 tracking-widest mb-4">
            Bob Worden's New Title
          </h3>

          <h1 class="font-semibold text-gray-700 mb-4">
            How to Stop Wars <br />and Save the World
          </h1>

          <h2>Lessons in Negotiation, Settlement, <br />and Leadership</h2>
        </div>

        <button
          class="text-white bg-yellow-500 py-2 px-8 uppercase tracking-wide shadow-lg font-bold"
          on:click={readMore}>Read More</button
        >
      </div>

      <div class="flex justify-end">
        <TriangleGraphic />
      </div>
    </div>
  </section>
</section>

<section id="read-more" class="bg-slate-800 p-12">
  <div
    class="page-content-width px-2 mx-auto grid grid-cols-3 gap-4 text-white"
  >
    <div class="p-4">
      <h2 class="font-semibold mb-4">
        Soon to be available on Amazon and booksellers everywhere.
      </h2>
      <hr class="h-px w-1/6 bg-white" />
    </div>

    <div class="p-4">
      Soon to be available on Amazon and booksellers everywhere. In this new
      short book, How to Stop Wars and Save the World, Bob Worden analyzes the
      conflicts which led to fighting three American wars. He reveals surprising
      stories which most people don’t know. Learn how to settle disputes of any
      kind, while learning the key facts and circumstances which ignited the
      Revolutionary, Civil and Vietnam wars. Using the mistakes leaders made in
      these conflicts,
    </div>

    <div class="p-4">
      Bob explains principles of settlement and negotiation, and demonstrates
      why settlement, if possible, is always preferable to going to war. Bob
      avoids unnecessary details and dates, and tells the stories behind the
      wars, captivating readers, who are fascinated to learn what these wars
      were all about, and why we need to settle, rather than fight, whenever
      possible.
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
