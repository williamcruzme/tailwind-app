<template>
  <button
    class="mx-2 font-light"
    :class="
      primary
        ? 'bg-black px-3 py-1 rounded-md text-white font-medium'
        : 'text-gray-700'
    "
  >
    <slot />
  </button>
</template>

<script>
export default {
  props: {
    primary: Boolean
  }
}
</script>
