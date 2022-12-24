<script>
	import '../app.css';
	import Navbar from '$lib/Navbar.svelte';
	import TabContent from '$lib/TabContent.svelte';
</script>

<Navbar tabs={['About Me', 'Projects', 'Contact']} />
<TabContent />
