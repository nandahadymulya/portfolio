<script setup>
const pageName = "Experience";
useSeoMeta({
  title: `${pageName} - Portfolio Nanda Hady Mulya`,
});

const experiences = [
  {
    company:
      "Peatland and Mangrove Restoration Agency of Republic of Indonesia",
    position: "Software Engineer",
    startDate: "Dec 2022",
    endDate: "Present",
  },
  {
    company: "PT Semen Padang",
    position: "IT Support Assistant Intern",
    startDate: "Mar 2022",
    endDate: "Aug 2022",
  },
  {
    company: "Laskar Negeri.id",
    position: "Manager of Design Creator",
    startDate: "Aug 2021",
    endDate: "Dec 2021",
  },
  {
    company: "PT Topik Sumbar Indonesia",
    position: "Wordpress Engineer",
    startDate: "Aug 2020",
    endDate: "Jan 2021",
  },
];
</script>
<template>
  <div class="mt-12 flex flex-col flex-wrap gap-3 justify-center">
    <div
      class="border border-zinc-100 hover:bg-teal-200 text-zinc-300 hover:text-zinc-500 text-xl text-center font-bold cursor-pointer p-2 rounded-lg transition-colors duration-300 ease-in-out"
    >
      Hire me!
    </div>
    <div
      v-for="experience in experiences"
      :key="experience.company"
      class="h-[4rem] w-[60rem]"
    >
      <div class="flex gap-3 rounded-lg h-full">
        <div class="bg-teal-500 w-1/5 p-2 rounded-lg text-zinc-100">
          {{ experience.startDate }} - {{ experience.endDate }}
        </div>
        <div class="bg-zinc-100 w-4/5 p-2 rounded-lg">
          <b>{{ experience.company }}</b>
          <p>
            <b> {{ experience.position }} </b>
          </p>
        </div>
        <!-- <div class="content-center bg-yellow-100 w-10 p-2 rounded-lg">></div> -->
      </div>
    </div>
  </div>
</template>
