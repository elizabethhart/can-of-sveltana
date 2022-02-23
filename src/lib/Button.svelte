<script lang="ts">
	export let style: string = 'primary';
	export let disabled: boolean = false;
	export let type: string = 'button';
</script>

<button {type} {disabled} class={style}><slot /></button>

<style>
	button {
		color: #fff;
		border: 0;
		border-radius: 8px;
		color: #fff;
		width: 200px;
		height: 60px;
		cursor: pointer;
	}

	.primary {
		background-color: #2d4085;
	}

	.secondary {
		background: #bcb4cc;
	}

	button:hover {
		transform: scale(0.98);
		opacity: 0.9;
	}

	button:disabled {
		background-color: #cccccc;
		color: #333;
		cursor: auto;
	}

	button:disabled:hover {
		transform: scale(1);
		opacity: 1;
	}
</style>
