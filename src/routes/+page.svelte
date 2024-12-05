<script>
	import '../css/main.css';
	import Navbar from './Navbar.svelte';
	import Body from './Body.svelte';

	let count = $state(0);

	let timers = $state([30, 10, 5]);
	let currentTimer = $state(0);

	function changeTimer(timer) {
		currentTimer = timer % timers.length;
	}

	function incrementCount() {
		count++;
	}
</script>

<Navbar {changeTimer} />

<Body {timers} {incrementCount} {currentTimer} {count} />
