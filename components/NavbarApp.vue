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
  <nav class="my-auto flex flex-wrap justify-center content-center w-screen gap-1 sm:gap-2 md:gap-3 p-3 sm:p-4 md:p-6">
    <div v-for="menu in menus" :key="menu.title">
      <NuxtLink :to="menu.to">
        <div :class="route.path === menu.to
          ? 'bg-teal-100 text-zinc-700 font-semibold '
          : 'bg-zinc-50 hover:bg-teal-50 text-zinc-500  hover:text-zinc-600 font-normal'
          " class="p-3 w-28 text-center text-sm rounded-lg transition-colors duration-500 ease-in-out cursor-pointer">
          {{ menu.title }}
        </div>
      </NuxtLink>
    </div>
  </nav>
</template>
