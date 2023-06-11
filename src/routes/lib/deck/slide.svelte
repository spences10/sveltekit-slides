<script lang='ts'>
  export let id: string | null = null
  export let animate=false
  export let restart=false

</script>

<section
  data-autoanimate-id={id}
  data-autoanimate={animate || null}
  data-autoanimate-restart={restart || null}
>
  <slot/>
</section>