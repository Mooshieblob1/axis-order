<script lang="ts">
	import '../app.css';
	let { children } = $props();
</script>

<!-- Full page background with Aqua borders -->
<div
	class="relative min-h-screen bg-white text-black"
	style="background-image: url('/images/aqua-border.png'), url('/images/aqua-border.png');
	       background-repeat: repeat-y, repeat-y;
	       background-position: left top, right top;
	       background-size: 2700px auto, 2700px auto;"
>
	<!-- Main centered content -->
	<div class="relative mx-auto w-full max-w-screen-xl bg-white px-4">
		<!-- Header -->
		<header
			class="flex items-center justify-between border-b border-gray-200 bg-white px-6 py-4 text-black"
		>
			<a href="/" class="flex shrink-0 items-center gap-4">
				<img src="/images/axislogo.png" alt="Axis Order" class="h-30 w-auto" />
			</a>

			<p class="mx-4 flex-1 text-center text-base font-medium text-gray-700">
				We make a living by what we get. But we make a life by what we give.
			</p>

			<a
				href="/join"
				class="shrink-0 rounded bg-blue-500 px-6 py-2 text-sm font-semibold tracking-wide text-white hover:bg-blue-600"
			>
				JOIN NOW
			</a>
		</header>

		<!-- Navbar -->
		<nav
			class="flex justify-center gap-6 border-b border-gray-200 bg-white py-4 text-sm font-medium text-black"
		>
			<a href="/" class="hover:text-blue-500 hover:underline">HOME</a>
			<a href="/who-we-are" class="hover:text-blue-500 hover:underline">WHO WE ARE</a>
			<a href="/anime" class="hover:text-blue-500 hover:underline">ANIMESTREAM!</a>
			<a href="/scoreboard" class="hover:text-blue-500 hover:underline">SCOREBOARD</a>
			<a href="/join" class="hover:text-blue-500 hover:underline">JOIN</a>
		</nav>

		<!-- Page content -->
		{@render children()}
	</div>
</div>
