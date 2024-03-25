<script>
  import { page } from '$app/stores';
</script>

<header>
  <div class="container page-content-width">
    <ul class="corner">
      <li aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
        <a href="/">Bob Worden, Esq.</a>
      </li>
    </ul>

    <nav>
      <ul>
        <li aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
          <a href="/" style="margin-right: 4rem">Home</a>
        </li>
        <li aria-current={$page.url.pathname === '/about' ? 'page' : undefined}>
          <a href="/about">About Bob</a>
        </li>
      </ul>
    </nav>
  </div>
</header>

<style>
  .container {
    width: 100%;
    display: flex;
    justify-content: space-between;
  }

  header {
    display: flex;
    justify-content: space-around;
    background-color: var(--color-white);
    border-bottom: 1px solid var(--color-gray-2);
    font-weight: 600;
  }

  li {
    list-style-type: none;
  }

  a {
    text-decoration: none;
    color: var(--color-black);
  }

  ul {
    display: flex;
    margin: 2rem 0rem;
    padding: 0;
  }

  .corner {
    text-transform: uppercase;
  }
</style>
