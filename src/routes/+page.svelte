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

<section class="flex">
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

<section id="read-more"></section>

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
