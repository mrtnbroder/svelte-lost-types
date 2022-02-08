<script lang="ts">
  /** CSS class for the element. */
  let _class: string | null = null
  export { _class as class }

  /** Whether the button is disabled. */
  export let disabled: boolean | null = null


</script>

<!-- when using $$restProps, the type infos get lost when running `svelte-kit package` -->
<!-- <button class={_class} {disabled} {...$$restProps}> -->
<button class={_class} {disabled}>
  <slot />
</button>
