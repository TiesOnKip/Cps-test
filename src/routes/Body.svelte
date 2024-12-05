<script>
	import '../css/main.css';
	import './Navbar.svelte';

	const { count, timers, currentTimer, incrementCount } = $props();
</script>

<div id="container">
	<h1 id="header">Cps test {timers[currentTimer]} seconds</h1>
	<h2 id="timer"></h2>
	<button id="cps-button" onclick={incrementCount}>Click me! <br /> {count}</button>
</div>
