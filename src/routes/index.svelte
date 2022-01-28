<script>
	import '../css/app.css';

	let cardNum = 1;
	let height = 0;

	let cards = [
		{ colour: '87ee11', name: 'lol' },
		{ colour: '5687ee', name: 'asldjf' }
	];
</script>

<svelte:window bind:outerHeight={height} />

<div class="fullscreen circles">
	{#each cards as card}
		<svg viewBox="0 0 {height} 768" class="circle"
			><g fill="#{card.colour}"
				><circle r={Math.floor(Math.random() * 300) + 150} cx="858" cy="339" /><circle
					r={Math.floor(Math.random() * 300) + 150}
					cx="241"
					cy="258"
				/><circle r={Math.floor(Math.random() * 300) + 150} cx="1365" cy="428" /><circle
					r={Math.floor(Math.random() * 250) + 150}
					cx="78"
					cy="745"
				/></g
			></svg
		>
	{/each}
</div>

<div class="fullscreen">
	<div class="wrapper">
		<h1>;lakjsdf</h1>
	</div>
</div>
