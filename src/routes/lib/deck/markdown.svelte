<script lang="ts">
	export let name = 'external.md'
	export let external = false
</script>

{#if external}
	<section data-markdown={name} />
{:else}
	<section data-markdown>
		<div data-template>
			<slot />
		</div>
	</section>
{/if}
