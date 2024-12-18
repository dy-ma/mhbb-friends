<script lang="ts">
	import '../app.css';
	let { children } = $props();

	import logo from '$lib/images/logo-primary.svg'
</script>

<!-- <header class="w-full p-2 bg-primary text-primary-foreground flex justify-between items-center">
	<a href="/">
		<img src={logo} alt="Temple Logo" class="size-16 invert" />
	</a>
	<nav>
		<ul class="flex p-2 font-serif">
			<li class="mx-2 hover:underline"><a href="#directions">Directions</a></li>
			<li class="mx-2 hover:underline"><a href="#contact">Contact</a></li>
		</ul>
	</nav>
</header> -->

<header class="w-full flex items-center justify-center absolute">
	<a href="/">
	<img src={logo} alt="Temple Logo" class="w-20 h-20 overflow-visible"></a>
</header>

{@render children()}