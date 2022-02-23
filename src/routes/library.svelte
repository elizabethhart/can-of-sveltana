<script context="module">
	import Button from '$lib/Button.svelte';
</script>

<svelte:head>
	<title>Library</title>
</svelte:head>

<div class="content">
	<section>
		<h2>Buttons</h2>
		<div class="content-item"><Button style="primary">Primary Button</Button></div>
		<div class="content-item"><Button style="secondary">Secondary Button</Button></div>
		<div class="content-item"><Button style="primary" disabled={true}>Disabled Button</Button></div>
	</section>
</div>

<style>
	.content {
		width: 100%;
		max-width: var(--column-width);
		margin: var(--column-margin-top) auto 0 auto;
		display: flex;
		flex-direction: column;
		justify-content: center;
	}

	.content-item {
		margin: 5px;
	}
</style>
