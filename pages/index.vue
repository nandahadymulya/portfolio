<script setup>
const pageName = "Dashboard";
useSeoMeta({
  title: `${pageName} - Portfolio Nanda Hady Mulya`,
});
</script>
<template>
  <div>
    <h2>
      Hi 👋, <br />
      <span> I'm Nanda Hady Mulya</span>.
    </h2>
    <div>
      A <b>Software Engineer</b> passionate about solving problems with tech.
      <br />
      I'm skilled in <b>Backend Development</b>, <b>Frontend Development</b>,
      and currently learning <b>Mobile Development</b>.
    </div>
    <div class="cta--container">
      <NuxtLink to="/project" class="btn--primary">Explore</NuxtLink>
      <NuxtLink to="/contact" class="btn--secondary">Get in touch</NuxtLink>
    </div>
    <!-- <div class="tech--stack--container"> -->
    <!-- Tech Stack -->
    <!-- <div class="tech--stack--item">Nuxt</div> -->
    <!-- </div> -->
  </div>
</template>
<style scoped>
h1,
h2 {
  font-size: 3rem;
  font-weight: 700;
  margin-bottom: 1rem;
}

.cta--container {
  margin: 1rem 0;
  display: flex;
  gap: 1rem;
}

.btn--primary {
  background-color: var(--color-primary);
  color: var(--color-light);
  padding: 0.75rem 1.5rem;
  border-radius: 1.25rem;
  transition: all 0.3s ease-in-out;
}

.btn--primary:hover {
  filter: drop-shadow(0 0 0.75rem var(--color-primary));
  transition: all 0.3s ease-in-out;
}

.btn--secondary {
  background-color: var(--color-light);
  border: 1px solid var(--color-primary);
  color: var(--color-primary);
  padding: 0.75rem 1.5rem;
  border-radius: 1.25rem;
  transition: all 0.3s ease-in-out;
}

.btn--secondary:hover {
  filter: drop-shadow(0 0 0.75rem var(--color-primary));
  transition: all 0.3s ease-in-out;
}
</style>
