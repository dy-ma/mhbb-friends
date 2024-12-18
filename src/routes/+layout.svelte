<script lang="ts">
	import '../app.css';
	let { children } = $props();

	import logo from '$lib/images/logo-primary.svg'
</script>

<header class="w-full flex items-center justify-center absolute">
	<a href="/">
	<img src={logo} alt="Temple Logo" class="w-20 h-20 overflow-visible"></a>
</header>

{@render children()}