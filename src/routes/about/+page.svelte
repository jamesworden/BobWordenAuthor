<script>
  import ProfileCard from '../ProfileCard.svelte';
  import TriangleGraphic from '../TriangleGraphic.svelte';
</script>

<svelte:head>
  <title>About</title>
  <meta name="description" content="About this app" />
</svelte:head>

<section class=""></section>

<!-- <section class="flex bw-page-content-width md:mx-auto w-full">
  <section class="bw-diagonal-bg py-8 pr-8 flex flex-1">
    <div class="py-16 bg-gray-50 flex flex-col justify-between flex-1">
      <div class="px-4">
        <div class="mb-12">
          <h3 class="uppercase text-gray-600 tracking-widest mb-4">
            Bob Worden, Esq.
          </h3>

          <h1
            class="font-semibold text-gray-700 mb-4 text-4xl sm:text-5xl md:text-6xl"
          >
            About Bob
          </h1>

          <h2>Award Winning Mediator and Arbitrator</h2>
        </div>
      </div>

      <div class="flex justify-end md:pr-16">
        <TriangleGraphic />
      </div>
    </div>
  </section>
</section> -->

<section
  id="read-more"
  class="bw-page-content-width mx-auto flex justify-between gap-x-4 w-full"
>
  <div class="flex-1 px-4">
    <div class="py-24">
      <h3 class="uppercase text-gray-600 tracking-widest mb-4">
        Bob Worden, Esq.
      </h3>

      <h1
        class="font-semibold text-gray-700 mb-4 text-4xl sm:text-5xl md:text-6xl"
      >
        About Bob
      </h1>

      <h2>Award Winning Mediator and Arbitrator</h2>
    </div>

    <p class="max-w-xl text-md md:max-w-2xl md:text-xl mb-8 md:mb-16">
      After decades of litigating in the Courts, representing individuals,
      insurance companies and corporations, Bob Worden became a Mediator,
      gratified to help settle lawsuits and eliminate the waste and pain of
      going to Court. Bob also became a reader of history, willing to wade
      through lengthy academic histories that bore most people, to find out what
      really happened that led to the fighting. Bob found that there were great
      similarities in the conflicts that led to these American wars with the
      conflicts that drive lawsuits. At the same time, recognizing that most
      people are turned off by the dates and events that they were forced to
      memorize in school, Bob wanted to share what he learned, to make it easy
      for his readers to know the key people, situations and the arguments which
      ignited the war of the Revolution, the Civil war and the Vietnam war. <br
      /><br /> Bob explains the stories of these wars in an entertaining, very readable
      way. Most readers will be happy to finally understand what these wars were
      all about. Observing that the political issues we deal with today are similar
      to those in dispute since America began, Bob explains the qualities which his
      readers should look for, to help choose better leaders going forward. How to
      Stop Wars and Save the World is a good choice for college-level courses and
      for anyone who wants to become better at resolving disputes early, avoiding
      unnecessary expense and the risks of continuing to fight. It is also a good
      choice for students who want an engaging way to learn about these American
      wars, providing the perspective missing in most textbooks.
    </p>
  </div>

  <div class="hidden md:block flex flex-col gap-y-8 flex-1">
    <div class="bw-diagonal-bg min-h-96 flex">
      <div class="m-8 bg-gray-50 flex-1 flex justify-end">
        <div class="flex flex-col justify-between m-8">
          <div class="flex-1"></div>
          <TriangleGraphic />
        </div>
      </div>
    </div>

    <div class="flex justify-around mt-8">
      <ProfileCard />
    </div>
  </div>
</section>
