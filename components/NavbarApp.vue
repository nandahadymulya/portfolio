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
  <nav class="menu--container">
    <div v-for="menu in menus" :key="menu.title">
      <NuxtLink
        :to="menu.to"
        :class="route.path === menu.to ? 'menu--item--active' : ''"
        class="menu--item"
      >
        {{ menu.title }}
      </NuxtLink>
    </div>
  </nav>
</template>
<style scoped>
.menu--container {
  display: flex;
  gap: 1rem;
}

.menu--item {
  color: var(--color-light);
  background-color: none;
  padding: 0.75rem;
  border-radius: 1.25rem;
}

.menu--item--active {
  background-color: var(--color-light);
  color: var(--color-primary);
  transition: all 0.3s ease-in-out;
}
</style>
