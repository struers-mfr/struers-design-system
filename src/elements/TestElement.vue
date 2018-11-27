<template>
  <div class="class">
    <slot/>
  </div>
</template>

<script>
/**
 * Used to build the outer wrapper of a page, including the page title and
 * associated actions. Wrapper doesn’t provide customizable options.
 */
export default {
  name: "TestElement",
  status: "prototype",
  release: "0.0.1",
  props: {
    /**
     * The html element name used for the wrapper.
     */
    type: {
      type: String,
      default: "div",
    },
  },
}
</script>

<style lang="sass" scoped>
.class
  +reset
  font-size: $size-m
  color: $color-ucla-gold
</style>


<docs>
  ```jsx
  <TestElement>Wrapper can be used to wrap any components together.</TestElement>
  ```
</docs>
