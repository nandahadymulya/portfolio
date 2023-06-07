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
  <nav
    class="my-auto h-20 flex flex-wrap justify-center content-center w-screen gap-3"
  >
    <div v-for="menu in menus" :key="menu.title">
      <NuxtLink :to="menu.to">
        <div
          :class="
            route.path === menu.to
              ? 'bg-teal-100 text-zinc-700 font-semibold '
              : 'bg-zinc-50 hover:bg-teal-50 text-zinc-500  hover:text-zinc-600 font-normal'
          "
          class="p-3 w-28 text-center text-sm rounded-lg transition-colors duration-300 ease-in-out cursor-pointer"
        >
          {{ menu.title }}
        </div>
      </NuxtLink>
    </div>
  </nav>
</template>
