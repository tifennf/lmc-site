<script>
	import '$src/styles.css';
	import 'carbon-components-svelte/css/g10.css';
</script>

<main>
	<nav>
		<h1><a class="home-link" href="/">Acceuil</a></h1>
		<h1>Guide Jussieu</h1>
		<ul>
			<li>
				<a href="/">Vocabulaires</a>
			</li>
			<li>
				<a href="/">Liens utiles</a>
			</li>
			<li>
				<a href="/">Plan</a>
			</li>
			<li>
				<a href="/">Cheat codes</a>
			</li>
		</ul>
		<h1>Assos Jussieu</h1>
		<ul>
			<li>
				<a href="/assos-matiere">Assos matière</a>
			</li>
			<li>
				<a href="/">Assos cursus</a>
			</li>
			<li>
				<a href="/">Assos art et jeux</a>
			</li>
			<li>
				<a href="/">Assos bde</a>
			</li>
		</ul>
	</nav>
	<article>
		<div>
			<slot />
		</div>
	</article>
</main>

<style>
	main {
		height: 100%;

		display: grid;
		grid-template-columns: 1fr 5fr;
		grid-auto-flow: column;
	}
	nav {
		display: flex;
		flex-direction: column;
		height: 100%;

		background-color: var(--nav-color);
		color: white;
		padding: 2rem;
		gap: 1rem;
	}

	article {
		padding: 2rem;
		display: grid;
		grid-template-columns: 1fr 4fr 1fr;
	}
	article > div {
		grid-column-start: 2;
	}
	h1 {
		font-size: var(--h1-size);
		margin: 0;
	}
	ul {
		display: flex;
		flex-direction: column;
		gap: 0.5rem;
	}

	a {
		text-decoration: none;
		color: unset;
	}

	ul a {
		font-size: var(--h3-size);
	}
	ul {
		margin: 0;
		padding: 0;
		list-style-type: none;
	}
	li {
		padding-left: 1rem;
	}
</style>
