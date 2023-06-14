<script lang="ts">
	import { onMount } from 'svelte'

	import Reveal from 'reveal.js'
	import Highlight from 'reveal.js/plugin/highlight/highlight'
	import Markdown from 'reveal.js/plugin/markdown/markdown'
	import Notes from 'reveal.js/plugin/notes/notes'

	import 'highlight.js/styles/night-owl.css'
	import 'reveal.js/dist/reveal.css'
	import 'reveal.js/dist/theme/white.css'
	import Presentation from './presentation.svelte'

	onMount(() => {
		const deck = new Reveal({
			autoAnimateEasing: 'ease',
			autoAnimateDuration: 0.3,
			hash: true,
			controls: true,
			progress: true,
		})

		deck.initialize({
			plugins: [Markdown, Highlight, Notes],
		})
	})
</script>

<div class="reveal">
	<div class="slides">
		<Presentation />
	</div>
</div>
