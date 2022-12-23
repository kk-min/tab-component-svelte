<script lang="ts">
	export let active = false;

	function onClick() {
		active = true;
	}
</script>

<button class="tab" on:click={onClick} class:active>
	<slot />
</button>

<style>
	.tab {
		cursor: pointer;
		border-right: 1px solid #ccc;
		border-bottom: 1px solid #ccc;
	}
	.active {
		cursor: default;
		border-bottom: none;
	}
</style>
