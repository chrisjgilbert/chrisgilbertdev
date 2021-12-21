<script>
	import '../app.css';

	import Nav from '../components/nav.svelte';
</script>

<main>
	<Nav />
	<slot />
</main>

<style>
	main {
		max-width: 1024px;
		margin: auto;
		padding: 0 var(--m-spacer);
	}
</style>
