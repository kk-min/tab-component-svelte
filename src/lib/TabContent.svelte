<script>
	import { activeTab } from './TabStore';
</script>

<container>
	<h1>
		{$activeTab === 'Home' ? 'Home' : $activeTab === 'Projects' ? 'Projects' : 'Contact'}
	</h1>
</container>

<style>
	container {
		margin-top: 3rem;
		display: flex;
		justify-content: center;
		align-items: center;
	}
</style>
