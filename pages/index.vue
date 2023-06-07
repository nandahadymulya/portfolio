<script setup>
useSeoMeta({
  title: `Portfolio - Nanda Hady Mulya`,
});
</script>
<template>
  <div>
    <div class="greeting--container">
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
    </div>
    <div class="cta--container">
      <NuxtLink to="/project" class="btn--primary">Explore</NuxtLink>
      <NuxtLink to="/contact" class="btn--secondary">Get in touch</NuxtLink>
    </div>
    <hr />
    <div class="social--icon--container">
      <icon-app class="social--icon" />
    </div>
  </div>
</template>
<style scoped>
.greeting--container {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

h2 {
  color: var(--color-dark);
  font-size: 3rem;
  font-weight: 800;
  margin-bottom: 1rem;
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
