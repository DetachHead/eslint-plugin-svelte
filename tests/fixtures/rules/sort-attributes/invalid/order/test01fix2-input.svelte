<script>
  import MyComponent from "./MyComponent.svelte"
  let data, comp, abc, def
  let foo, bar
  let src
  const color = "red"
  function name() {}
  function fn() {}
</script>

<MyComponent data-foo bind:this={comp} bind:data {abc} {def} />
<input
  id="foo"
  class="my-block"
  class:bar
  value="abc"
  style:color
  bind:this={foo}
  style="width: 30px;"
  data-value="x"
  animate:name
  in:fn
  out:fn
  transition:fn
/>
<img id="bar" {src} alt="bar" />
