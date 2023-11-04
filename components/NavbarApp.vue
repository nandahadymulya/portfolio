<script setup>
const route = useRoute();

const menus = [
  { to: "/", title: "Home" },
  { to: "/experience", title: "Experience" },
  { to: "/project", title: "Project" },
  { to: "/education", title: "Education" },
  { to: "/about", title: "About" },
  { to: "/contact", title: "Contact Me" },
];
</script>
<template>
  <nav class="w-full sticky top-0 bg-white backdrop-blur-lg bg-filter bg-opacity-30 border-b border-zinc-100 z-2 my-auto p-3 sm:p-4 md:p-6
   ">
    <div class="hidden md:flex flex-wrap justify-center md:gap-2 md:gap-4">
      <NuxtLink :to="menu.to" v-for="menu in menus" :key="menu.title">
        <div :class="route.path === menu.to
          ? 'bg-teal-100 text-zinc-700 font-semibold'
          : 'bg-zinc-50 hover:bg-teal-50 text-zinc-500  hover:text-zinc-600 font-normal'
          " class="p-3 w-28 text-center text-sm rounded-lg transition-colors duration-500 ease-in-out cursor-pointer">
          {{ menu.title }}
        </div>
      </NuxtLink>
    </div>

    <div class="flex gap-2 items-center md:hidden">
      <button
        class="bg-zinc-50 text-zinc-500 font-semibold p-3 rounded-lg transition-colors duration-500 ease-in-out hover:bg-teal-100 hover:text-zinc-700">
        <Icon name="heroicons-solid:menu" color="#393e46" height="24" width="24" />
      </button>
      <h1 class="font-bold text-xl">Portfolio</h1>
    </div>
  </nav>
</template>
