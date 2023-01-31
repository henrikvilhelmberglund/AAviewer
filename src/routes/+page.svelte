<script>
	let fontSize = 16;
	$: lineHeight = fontSize + 2;
	let fonts = ["aahub_light4", "MSPGothic"];
	// TODO make sure the names are correct
	let activeStyle;
</script>

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
{fontSize}
<input type="range" name="fontsize" id="" bind:value={fontSize} min="10" max="24" />
{lineHeight}
<input type="range" name="lineheight" id="" bind:value={lineHeight} min="12" max="26" />

<br />

<textarea
	style="font-size: {fontSize + 'px'}; line-height: {lineHeight + 'px'};"
	class="font"
	name=""
	id="aa"
	cols="100"
	rows="70"
/>

<style>
	@font-face {
		font-family: "aahub_light4";
		src: url("$lib/fonts/aahub_light4.woff2") format("woff2"),
			url("$lib/fonts/aahub_light4.woff") format("woff"),
			url("$lib/fonts/aahub_light4.ttf") format("ttf");
		font-display: swap;
	}

	.font {
		font-family: "aahub_light4", "MS PGothic";
		white-space: pre;
	}
</style>
