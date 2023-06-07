<template>
  <div class="w-screen h-screen p-2">
    <div class="sticky top-0 bg-white">
      <navbar-app />
    </div>
    <div class="flex justify-center items-center rounded-lg">
      <slot />
    </div>

    <div class="fixed bottom-0">
      <footer-app />
    </div>
  </div>
</template>
