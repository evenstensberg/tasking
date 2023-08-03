<script>
	const tasks = [
		{
			priority: 1.2,
			description: 'Go to work at 10:00 and finish 18:00'
		},
		{
			priority: 4.2,
			description: 'Exercise 30 minutes'
		},
		{
			priority: 2.9,
			description: 'Read a book'
		},
		{
			priority: 5.0,
			description: 'Morning coffee'
		}
	];
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<div class="main">
	{#each tasks as task}
		<div class="task-container">
			<div class="priority-container">
				<span class="priority-text">{task.priority}</span>
			</div>
			<div class="description-container">
				<span>{task.description}</span>
			</div>
		</div>
	{/each}
</div>

<style>
	.priority-text {
		font-size: 60px;
		color: white;
	}
	.priority-container {
		height: auto;
		width: 10%;
		display: grid;
		justify-content: center;
		align-items: center;
		background-color: rgb(94, 108, 129);
		border-radius: 1em;
	}
	.description-container {
		height: auto;
		width: 90%;
		display: grid;
		justify-content: start;
		align-items: center;
		margin-left: 10px;
		color: white;
		background-color: rgb(94, 108, 129);
		border-radius: 1em;
	}
	.main {
		width: 97%;
		height: auto;
		margin-left: 3em;
	}
	.task-container {
		display: flex;
		width: 100%;
		height: 10em;
		margin-top: 2em;
	}
	.description-container > span {
		padding: 2em;
		font-size: 30px;
	}

	h1 {
		width: 100%;
	}
</style>
