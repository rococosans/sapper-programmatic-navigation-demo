<script>
	import { goto } from '@sapper/app';
</script>

<style>
	h1, figure {
		text-align: center;
		margin: 0 auto;
	}

	h1 {
		font-size: 2.8em;
		text-transform: uppercase;
		font-weight: 700;
		margin: 0 0 0.5em 0;
	}

	figure {
		margin: 0 0 1em 0;
	}

	img {
		width: 100%;
		max-width: 400px;
		margin: 0 0 1em 0;
	}

	@media (min-width: 480px) {
		h1 {
			font-size: 4em;
		}
	}

	button {
		display: block;
    text-align: right;
    background-color: rgb(255, 62, 0);
    padding: 0.5em 1.8em 0.5em 1em;
    border-radius: .4rem;
    color: white;
    position: relative;
		text-decoration: none;
    cursor: pointer;
		border: none;
		font-size: 16px;
		margin: 0 auto;
	}
</style>

<svelte:head>
	<title>Sapper project template</title>
</svelte:head>

<h1>Great success!</h1>

<figure>
	<img alt='Borat' src='great-success.png'>
	<figcaption>HIGH FIVE!</figcaption>
</figure>

<button on:click={() => goto('/about')}>Go To About</button>
