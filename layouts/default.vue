<template>
  <div class="flex flex-col h-screen">

    <navbar-app class="flex-none header sticky bg-white" />

    <div class="flex-grow overflow-y-auto">
      <slot />
    </div>

    <footer-app class="flex-none footer" />
  </div>
</template>
