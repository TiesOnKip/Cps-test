<script>
	import '../css/main.css';
	import './Body.svelte';

	const { changeTimer } = $props();
</script>

<nav>
	<button onclick={() => changeTimer(5)}>5 sec</button>
	<button onclick={() => changeTimer(10)}>10 sec</button>
	<button onclick={() => changeTimer(30)}>30 sec</button>
</nav>
