<script lang="ts">
	import { onMount } from 'svelte';

	let audioRef: HTMLAudioElement;
	let playing: boolean = false;
	function play() {
		audioRef.play();
		playing = true;
	}
	onMount(() => {
		window.addEventListener('click', play);
		window.addEventListener('keydown', play);
	});
</script>

<div
	class="flex-grow flex flex-col items-center justify-center"
	style={!playing ? 'cursor: pointer;' : 'cursor: auto;'}
>
	<audio bind:this={audioRef} class="hidden" src="hello.mp3" preload="auto" autoplay />
	<div class="w-64 h-64">
		<img src="whosippin.gif" alt="i love reign okay who sippin today though" />
	</div>
</div>
<svelte:head>
	<title>i love reign energy</title>
	<meta name="title" content="i love reign energy" />
	<meta name="description" content="regin energ" />

	<!-- Open Graph / Facebook -->
	<meta property="og:type" content="website" />
	<meta property="og:url" content="https://reign.energy/" />
	<meta property="og:title" content="i love reign energy" />
	<meta property="og:description" content="regin energ" />
	<meta property="og:image" content="https://reign.energy/whosippin.gif" />

	<!-- Twitter -->
	<meta property="twitter:card" content="summary_large_image" />
	<meta property="twitter:url" content="https://reign.energy/" />
	<meta property="twitter:title" content="i love reign energy" />
	<meta property="twitter:description" content="regin energ" />
	<meta property="twitter:image" content="https://reign.energy/whosippin.gif" />
</svelte:head>
