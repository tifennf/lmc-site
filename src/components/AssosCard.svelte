<script>
	import { Tile, OutboundLink } from 'carbon-components-svelte';
</script>

<Tile>
	<h2 class="title">Association Mathématique Sorbonne Universite (AMSU)</h2>
	<div class="link-list">
		<div class="bar">
			<OutboundLink href="https://www.youtube.com/watch?v=oT0mkKCcSMo"
				>Vidéo de présentation</OutboundLink
			>
		</div>
		<div class="bar">
			<OutboundLink href="https://discord.gg/Ja7CQvKnne">Discord</OutboundLink>
		</div>
		<div class="bar">
			<OutboundLink href="https://www.amsu.fr/">Site</OutboundLink>
		</div>
		<div class="bar">
			<OutboundLink href="http://facebook.com/amsu.fr">Facebook</OutboundLink>
		</div>
		<div class="bar">
			<OutboundLink href="https://www.instagram.com/amsujussieu/">Instagram</OutboundLink>
		</div>
		<div class="mail">contacteramsu@gmail.com</div>
	</div>
</Tile>

<style>
	.link-list {
		padding: 1rem;
		padding-left: 1.5rem;
		display: flex;
		flex-direction: column;
		gap: 1rem;
		position: relative;
	}

	.mail {
		padding: 0.5rem;
		background-color: hsl(0, 0%, 90%);
		border-style: solid;
		position: absolute;
		top: 0;
		right: 0;
	}

	.title {
		border-bottom-style: solid;
		border-bottom-width: 1px;
	}
	h2 {
		font-size: var(--h2-size);
	}
</style>
