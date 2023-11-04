<script setup>
useSeoMeta({
  title: `Portfolio - Nanda Hady Mulya`,
});

const skills = [
  { code: 'HTML' }, { code: 'CSS' }, { code: 'SCSS/SASS' },
  { code: 'Tailwind' }, { code: 'JavaScript' }, { code: 'TypeScript' },
  { code: 'PHP' }, { code: 'Python' }, { code: 'Dart' }, { code: 'Go' },
  { code: 'MySQL' }, { code: 'PostgreSQL' }, { code: 'SQLite' }, { code: 'MongoDB' },
  { code: 'Docker' },
]
</script>
<template>
  <div class="flex flex-col p-6 md:p-16">
    <main class="bg-zinc-50 p-10 rounded-2xl mb-6">
      <div class="mb-12">
        <h2 class="font-extrabold text-3xl sm:text-4xl md:text-5xl text-zinc-700 leading-relaxed">
          Hi 👋, <br />
          <span class=""> I'm Nanda Hady Mulya</span>.
        </h2>
        <div class="my-3 text-zinc-700 leading-relaxed">
          A <b>Software Engineer</b> has a sense of design and experienced full-stack development specializing in
          <b>Python</b>, <b>TypeScript</b>, and <b>Flutter</b>.
          I am interested in <b>Natural Language Processing</b> and <b>Machine Learning (ML)</b>.
        </div>
      </div>
      <div class="flex gap-3 my-3">
        <NuxtLink to="/project"
          class="bg-teal-500 hover:bg-teal-700 text-zinc-100 hover:text-zinc-50 font-normal text-center rounded-lg p-2 w-32 ease-in-out duration-500 delay-75">
          Explore</NuxtLink>
        <NuxtLink to="/contact"
          class="bg-white text-teal-500 hover:text-teal-700 border border-teal-500 hover:border-teal-700 font-normal text-center border-solid  rounded-lg p-2 w-32 ease-in-out duration-500 delay-75">
          Get in touch</NuxtLink>
      </div>
      <hr class="my-3" />
      <div class="my-3">
        <icon-app />
      </div>
    </main>


    <section class="justify-center items-center">
      <h3 class="text-2xl font-semibold text-teal-500 mb-6">Skills</h3>
      <div class="flex justify-center flex-wrap gap-3">
        <div v-for="item in skills" :key="item.code">
          <div
            class="bg-zinc-50 border border-transparent hover:border-teal-500 hover:text-teal-500 px-6 py-4 rounded ease-in-out duration-500 delay-75">
            {{
              item.code }}
          </div>
        </div>
      </div>
    </section>
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
