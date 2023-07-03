<script lang="ts">
	import { invoke } from '@tauri-apps/api/tauri';

	async function greet() {
		await invoke('open_docs');
	}
</script>

<button on:click="{greet}">Live</button>
<button>Stop</button>

<style lang="postcss">
	:global(html) {
		background-color: theme(colors.gray.100);
	}
</style>
