<template>
  <div>
    <!-- Using utilities -->
    <button class="px-4 py-2 font-bold text-white bg-blue-500 rounded hover:bg-blue-700">
      Button
    </button>

    <!-- Extracting classes using @apply -->
    <button class="btn btn-blue">
      Button
    </button>
  </div>
</template>

<style>
  .btn {
    @apply px-4 py-2 rounded font-bold;
  }
  .btn-blue {
    @apply text-white bg-blue-500;
  }
  .btn-blue:hover {
    @apply bg-blue-700;
  }
</style>
