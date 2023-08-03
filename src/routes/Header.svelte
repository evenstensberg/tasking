<script>
	import { page } from '$app/stores';
	import logo from '$lib/images/svelte-logo.svg';
	import github from '$lib/images/github.svg';
</script>

<header>
	<div class="tasking-container">
		<p class="tasking-name">TASKING</p>
	</div>
</header>

<style>
	header {
		display: flex;
		justify-content: space-between;
	}

	.tasking-container {
		margin-top: 1em;
		border: 2px solid white;
		width: 20em;
		height: 10em;
		border-top-right-radius: 5em;
		border-bottom-right-radius: 5em;
		background-color: white;
	}

	.tasking-name {
		display: flex;
		justify-content: center;
		width: 100%;
		height: 100%;
		font-size: 50px;
		color: red;
	}

	a:hover {
		color: var(--color-theme-1);
	}
</style>
