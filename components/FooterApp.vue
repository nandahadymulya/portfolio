<script setup>
const date = new Date();
const year = date.getFullYear();
</script>
<template>
  <footer class="w-full p-2 sm:p-3 md:p-4 bg-zinc-100 text-zinc-500 text-base text-center">
    &copy; {{ year }} - Nanda Hady Mulya. All rigth reserved.
  </footer>
</template>
