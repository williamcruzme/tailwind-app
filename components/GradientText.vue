<template>
  <span :class="`relative bg-clip-text bg-gradient-to-r ${from} ${to}`">
    <slot />
  </span>
</template>

<script>
export default {
  props: {
    from: {
      type: String,
      required: true
    },
    to: {
      type: String,
      required: true
    }
  }
}
</script>
