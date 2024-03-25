<script>
  import ProfileCard from './ProfileCard.svelte';
</script>

<svelte:head>
  <title>Home</title>
  <meta
    name="description"
    content="Bob Worden's Latest Title, How to Stop Wars and Save the World"
  />
</svelte:head>

<section class="flex">
  <ProfileCard />

  <div class="diagonal-bg p-8">
    <div class="p-16 pb-48 bg-gray-50">
      <div class="mb-12">
        <h3 class="uppercase text-gray-600 tracking-widest">
          Bob Worden's New Title
        </h3>

        <h1>How to Stop Wars and Save the World</h1>

        <h2>Lessons in Negotiation, Settlement, and Leadership</h2>
      </div>

      <button
        class="text-white bg-amber-500 py-2 px-8 uppercase tracking-wide shadow-lg font-bold"
        >Read More</button
      >
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
