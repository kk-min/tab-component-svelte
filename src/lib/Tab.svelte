<script lang="ts">
	import { activeTab } from './TabStore';
	export let tabName: string = '';
	function onClick() {
		activeTab.set(tabName);
	}
</script>

<button class="tab" on:click={onClick} class:active={$activeTab === tabName}>
	{tabName}
</button>

<style>
	.tab {
		cursor: pointer;
		border: 0;
		border-right: 1px solid var(--color-inactive);
		border-bottom: 1px solid var(--color-inactive);
		background: none;
		box-shadow: none;
		border-radius: 0;
		min-height: 8vh;
		font-size: 1.5em;
		padding: 15px 5vw 15px 5vw;
		color: var(--color-inactive);
	}
	.tab:hover {
		color: var(--color-secondary);
	}
	.active {
		cursor: default;
		font-weight: bold;
		border-top: 5px solid var(--color-primary);
		border-bottom: none;
		color: var(--color-secondary);
		padding: 10px 5vw 15px 5vw;
	}
</style>
