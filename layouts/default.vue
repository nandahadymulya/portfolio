<template>
  <div class="flex flex-col h-screen">

    <navbar-app class="flex-none" />

    <div class="flex-grow flex-col p-6 md:p-16">
      <slot />
    </div>

    <footer-app class="flex-none" />
  </div>
</template>
