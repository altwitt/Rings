<script>
	import Header from './Header.svelte';
	import './styles.css';
	import pus from '$lib/images/pus.gif';
</script>

<div class="app">
	<Header />

	<main>
		<slot />
	</main>

	<footer>
		<p>RECOGNIZE ANY UNNAMED ARTISTS IN MASHUPS? <span><img src={pus} alt="PussNBoots" /></span> I WOULD LOVE TO KNOW, PLEASE.</p>
	</footer>
</div>

<style>
	:global(body) {
		margin: 0;
		padding: 1rem;
	}
	
	:global(p) {
		font-size: 12px;
	}
	
	:global(strong) {
		font-size: 14px;
	}
	
	:global(button) {
		font-size: 14px;
	}
	
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}

	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 64rem;
		margin: 0 auto;
		box-sizing: border-box;
	}
P {
	font-size: 16px;
	font-style: italic;
	font-weight: 900;

}
	footer {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding: 12px;
	}

	img {
		width: 4em;
		height: 4em;
		object-fit: contain;
	}

	@media (min-width: 480px) {
		footer {
			padding: 12px 0;
		}
	}
</style>
