<script lang="ts">
	import Code from './code.svelte'
	import Markdown from './markdown.svelte'
	import Notes from './notes.svelte'
	import Slide from './slide.svelte'
</script>

<Slide animate>
	<h1>Slide 1</h1>
</Slide>

<Slide animate>
	<h1>Slide 2</h1>
</Slide>

<Slide animate>
	<h2>With notes</h2>
	<p>Press <code>s</code></p>
	<Code>
		{`
      const a = 1
      const b = 2
      const c = a + b
    `}
	</Code>
	<Notes>
		<h1>Notes for slide 3</h1>
		<p>These are the notes for slide 3</p>
	</Notes>
</Slide>

<Markdown>
	{`
    # Slide 3

    - list item 1
    - list item 2
    - list item 3
  `}
</Markdown>

<Markdown name="slides.md" external />
