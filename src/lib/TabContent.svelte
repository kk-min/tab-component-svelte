<script>
	import { activeTab } from './TabStore';
</script>

<h1>
	{$activeTab === 'Home' ? 'Home' : $activeTab === 'Projects' ? 'Projects' : 'Contact'}
</h1>
