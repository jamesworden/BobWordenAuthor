<script>
	import { page } from '$app/stores';
</script>

<header>
	<div class="container">
		<ul class="corner">
			<li aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
				<a href="/">Bob Worden, Esq.</a>
			</li>
		</ul>
	
		<nav>
			<ul>
				<li aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
					<a href="/">Home</a>
				</li>
				<li aria-current={$page.url.pathname === '/about' ? 'page' : undefined}>
					<a href="/about">About Bob</a>
				</li>
			</ul>
		</nav>
	</div>
</header>

<style>
	header {
		display: flex;
		justify-content: space-around;
		background-color: var(--color-white-0);
		border-bottom: 1px solid var(--color-gray-2);
		font-weight: 600;
	}

	li {
		list-style-type: none;
		margin-right: 4rem
	}

	a {
		text-decoration: none;
		color: var(--color-black);
	}

	ul {
		display: flex;
		margin: 2rem;
	}

	.corner {
		text-transform: uppercase;
	}
</style>
