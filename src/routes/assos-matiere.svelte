<script>
	import { Tile, OutboundLink } from 'carbon-components-svelte';
	import AssosCard from '$src/components/AssosCard.svelte';
</script>

<div class="wrapper">
	<AssosCard />
	<AssosCard />
</div>

<style>
	.wrapper {
		display: flex;
		flex-direction: column;
		gap: 2rem;
		padding: 0 1rem;
	}
</style>
