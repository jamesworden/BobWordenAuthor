<script>
  import Header from './Header.svelte';
  import Footer from './Footer.svelte';
  import './styles.css';
</script>

<div class="flex flex-col min-h-screen">
  <Header />

  <main class="flex flex-col w-full flex-1 mx-auto box-border">
    <slot />
  </main>

  <Footer />
</div>
