<script lang="ts">
	import '../app.postcss'
	import Slides from './lib/deck/slides.svelte'
</script>

<Slides />

<style>
	:global(:root) {
		--r-main-font: 'Poppins';
		--r-heading-font: 'Manrope';
		--r-code-font: 'Victor Mono';
		--r-heading-text-transform: none;
	}
</style>
