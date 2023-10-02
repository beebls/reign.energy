<script>
	import '../app.css';
</script>

<div class="bg-black w-screen min-h-screen flex flex-col">
	<slot />
</div>
<svelte:head>
	<!-- Primary Meta Tags -->
	<title>i love reign energy</title>
	<meta name="title" content="i love reign energy" />
	<meta name="description" content="regin energ" />

	<!-- Open Graph / Facebook -->
	<meta property="og:type" content="website" />
	<meta property="og:url" content="https://reign.energy/" />
	<meta property="og:title" content="i love reign energy" />
	<meta property="og:description" content="regin energ" />
	<meta property="og:image" content="reign.gif" />

	<!-- Twitter -->
	<meta property="twitter:card" content="summary_large_image" />
	<meta property="twitter:url" content="https://reign.energy/" />
	<meta property="twitter:title" content="i love reign energy" />
	<meta property="twitter:description" content="regin energ" />
	<meta property="twitter:image" content="reign.gif" />
</svelte:head>
