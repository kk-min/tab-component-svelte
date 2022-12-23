<script lang="ts">
	import { activeTab } from './TabStore';
	export const tabName = '';
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
		border-right: 1px solid var(--color-inactive);
		border-bottom: 1px solid var(--color-inactive);
	}
	.active {
		cursor: default;
		border-top: 1px solid var(--color-primary);
		border-bottom: none;
		color: var(--color-secondary);
	}
</style>
