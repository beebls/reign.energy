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
	<audio bind:this={audioRef} class="hidden" src="tron.mp3" preload="auto" autoplay />
	<div class="w-64 h-64">
		<img src="orangedreamsicle.gif" alt="orange dreamsicle reign" />
	</div>
</div>
