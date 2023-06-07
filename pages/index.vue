<script setup>
useSeoMeta({
  title: `Portfolio - Nanda Hady Mulya`,
});
</script>
<template>
  <div class="flex flex-col mt-40">
    <div class="">
      <h2 class="font-extrabold text-5xl text-zinc-700 leading-relaxed">
        Hi 👋, <br />
        <span class=""> I'm Nanda Hady Mulya</span>.
      </h2>
      <div class="my-3 text-zinc-700 leading-relaxed">
        A <b>Software Engineer</b> passionate about solving problems with tech.
        <br />
        I'm skilled in <b>Backend Development</b>, <b>Frontend Development</b>,
        and currently learning <b>Mobile Development</b>.
      </div>
    </div>
    <div class="flex gap-3 my-3">
      <NuxtLink
        to="/project"
        class="bg-teal-500 hover:bg-teal-700 text-zinc-100 font-normal text-center rounded-lg p-2 w-32 transition-colors duration-300 ease-in-out"
        >Explore</NuxtLink
      >
      <NuxtLink
        to="/contact"
        class="bg-white text-teal-500 hover:text-teal-700 font-normal text-center border-solid border border-teal-500 hover:border-teal-700 rounded-lg p-2 w-32 transition-colors duration-300 ease-in-out"
        >Get in touch</NuxtLink
      >
    </div>
    <hr class="my-3" />
    <div class="my-3">
      <icon-app />
    </div>
  </div>
</template>
<style scoped>
.greeting--container {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.cta--container,
.social--icon--container {
  display: flex;
  gap: 1rem;
  margin: 1rem 0;
}

.btn--primary {
  background-color: var(--color-primary);
  border-radius: 1.25rem;
  color: var(--color-light);
  padding: 0.75rem 1.5rem;
  transition: all 0.3s ease-in-out;
}

.btn--primary:hover {
  filter: drop-shadow(0 0 0.75rem var(--color-primary));
  transition: all 0.3s ease-in-out;
}

.btn--secondary {
  background-color: var(--color-light);
  border: 1px solid var(--color-primary);
  border-radius: 1.25rem;
  color: var(--color-primary);
  padding: 0.75rem 1.5rem;
  transition: all 0.3s ease-in-out;
}

.btn--secondary:hover {
  filter: drop-shadow(0 0 0.75rem var(--color-primary));
  transition: all 0.3s ease-in-out;
}
</style>
