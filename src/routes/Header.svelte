<script>
  import { page } from '$app/stores';
</script>

<header class="flex justify-around font-semibold">
  <div class="w-full flex justify-between page-content-width p-2">
    <ul class="uppercase list-none my-3 p-0">
      <li aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
        <a href="/" class="no-underline">Bob Worden, Esq.</a>
      </li>
    </ul>

    <nav>
      <ul class="list-none flex my-3 p-0">
        <li aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
          <a href="/" class="no-underline mr-16">Home</a>
        </li>
        <li aria-current={$page.url.pathname === '/about' ? 'page' : undefined}>
          <a href="/about" class="no-underline">About Bob</a>
        </li>
      </ul>
    </nav>
  </div>
</header>

<style>
  header {
    background-color: var(--color-white);
    border-bottom: 1px solid var(--color-gray-2);
  }

  a {
    color: var(--color-black);
  }
</style>
