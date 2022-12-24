<script>
	import Tab from './Tab.svelte';
	const tabs = ['Home', 'Projects', 'Contact'];
</script>

<div class="navbar">
	{#each tabs as tab}
		<Tab tabName={tab} />
	{/each}
	<div class="filler" />
</div>

<style>
	.navbar {
		display: flex;
		position: fixed;
		top: 0;
		left: 0;
		width: 100%;
		max-height: 10vh;
		justify-content: flex-start;
		padding: 0;
	}
	.filler {
		display: flex;
		align-items: center;
		height: inherit;
		flex-grow: 1;
		border-bottom: 1px solid var(--color-inactive);
	}
</style>
