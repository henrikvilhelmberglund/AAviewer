<script>
	let fonts = [
		"aahub",
		"aahub_light",
		"aahub_light4",
		"monapo",
		"Saitamaar",
		"saitamaar_light",
		"RobotoJAA",
		"textar",
		"textar-min",
		"ume-pgc4",
		"monaya"
	];
  // TODO make sure the names are correct
	let activeStyle;
</script>

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

{#each fonts as font}
	<button on:click={() => (activeStyle = font)}>{font}</button>
{/each}

<br />

<textarea class={activeStyle} name="" id="aa" cols="100" rows="70" />

<style>
	@font-face {
		font-family: "aahub";
		src: url("$lib/fonts/aahub.woff2") format("woff2"), url("$lib/fonts/aahub.woff") format("woff"),
			url("$lib/fonts/aahub.ttf") format("ttf");
		font-display: swap;
	}

	.aahub {
		font-family: "aahub";
		white-space: pre;
		font-size: 16px;
		line-height: 18px;
	}

	@font-face {
		font-family: "aahub_light";
		src: url("$lib/fonts/aahub_light.woff2") format("woff2"),
			url("$lib/fonts/aahub_light.woff") format("woff"),
			url("$lib/fonts/aahub_light.ttf") format("ttf");
		font-display: swap;
	}

	.aahub_light {
		font-family: "aahub_light";
		white-space: pre;
		font-size: 16px;
		line-height: 18px;
	}

	@font-face {
		font-family: "aahub_light4";
		src: url("$lib/fonts/aahub_light4.woff2") format("woff2"),
			url("$lib/fonts/aahub_light4.woff") format("woff"),
			url("$lib/fonts/aahub_light4.ttf") format("ttf");
		font-display: swap;
	}

	.aahub_light4 {
		font-family: "aahub_light4";
		white-space: pre;
		font-size: 16px;
		line-height: 18px;
	}

	@font-face {
		font-family: "monapo";
		src: url("$lib/fonts/monapo.woff2") format("woff2"),
			url("$lib/fonts/monapo.woff") format("woff"), url("$lib/fonts/monapo.ttf") format("ttf");
		font-display: swap;
	}

	.monapo {
		font-family: "monapo";
		white-space: pre;
		font-size: 16px;
		line-height: 18px;
	}

	@font-face {
		font-family: "Saitamaar";
		src: url("$lib/fonts/Saitamaar.woff2") format("woff2"),
			url("$lib/fonts/Saitamaar.woff") format("woff"), url("$lib/fonts/Saitamaar.ttf") format("ttf");
		font-display: swap;
	}

	.Saitamaar {
		font-family: "Saitamaar";
		white-space: pre;
		font-size: 16px;
		line-height: 18px;
	}

	@font-face {
		font-family: "saitamaar_light";
		src: url("$lib/fonts/saitamaar_light.woff2") format("woff2"),
			url("$lib/fonts/saitamaar_light.woff") format("woff"),
			url("$lib/fonts/saitamaar_light.ttf") format("ttf");
		font-display: swap;
	}

	.saitamaar_light {
		font-family: "saitamaar_light";
		white-space: pre;
		font-size: 16px;
		line-height: 18px;
	}

	@font-face {
		font-family: "RobotoJAA";
		src: url("$lib/fonts/RobotoJAA.woff2") format("woff2"),
			url("$lib/fonts/RobotoJAA.woff") format("woff"), url("$lib/fonts/RobotoJAA.ttf") format("ttf");
		font-display: swap;
	}

	.RobotoJAA {
		font-family: "RobotoJAA";
		white-space: pre;
		font-size: 16px;
		line-height: 18px;
	}

	@font-face {
		font-family: "textar";
		src: url("$lib/fonts/textar.woff2") format("woff2"),
			url("$lib/fonts/textar.woff") format("woff"), url("$lib/fonts/textar.ttf") format("ttf");
		font-display: swap;
	}

	.textar {
		font-family: "textar";
		white-space: pre;
		font-size: 16px;
		line-height: 18px;
	}

	@font-face {
		font-family: "textar-min";
		src: url("$lib/fonts/textar-min.woff2") format("woff2"),
			url("$lib/fonts/textar-min.woff") format("woff"),
			url("$lib/fonts/textar-min.ttf") format("ttf");
		font-display: swap;
	}

	.textar-min {
		font-family: "textar-min";
		white-space: pre;
		font-size: 16px;
		line-height: 18px;
	}

	@font-face {
		font-family: "ume-pgc4";
		src: url("$lib/fonts/ume-pgc4.woff2") format("woff2"),
			url("$lib/fonts/ume-pgc4.woff") format("woff"), url("$lib/fonts/ume-pgc4.ttf") format("ttf");
		font-display: swap;
	}

	.ume-pgc4 {
		font-family: "ume-pgc4";
		white-space: pre;
		font-size: 16px;
		line-height: 18px;
	}

	@font-face {
		font-family: "monaya";
		src: url("$lib/fonts/monaya.woff2") format("woff2"),
			url("$lib/fonts/monaya.woff") format("woff"), url("$lib/fonts/monaya.ttf") format("ttf");
		font-display: swap;
	}

	.monaya {
		font-family: "monaya";
		white-space: pre;
		font-size: 16px;
		line-height: 18px;
	}
</style>
