<template>
  <section id="services" class="relative text-white mt-32">
    <SectionHeader title="My Services" />
    <div
      class="mt-20 py-8 xl:px-16 px-4 sm:py-16 grid grid-cols-1 gap-6 pt-10 sm:grid-cols-2 md:gap-10 md:pt-12 lg:grid-cols-3"
    >
      <article
        class="px-[12px] mb-[24px]"
        v-for="element in services"
        :key="element.id"
      >
        <div
          class="mt-[30px] relative flex flex-col justify-center text-center rounded-[30px] border border-secondary dark:bg-[#FFFFFF29] bg-primary"
          data-aos="fade-up"
          :data-aos-delay="element.id * 100"
        >
          <div class="mt-[-30px] flex justify-center relative">
            <div class="mt-[-7px] p-[20px] relative bg-primary rounded-[50%]">
              <span
                class="h-[60px] w-[60px] m-auto border-[1px] border-solid border-secondary absolute top-[8px] left-[8px] rounded-[50px] inline-block z-[5]"
              ></span>
              <img
                :src="element.icon"
                alt="services"
                class="h-[35px] w-[35px] relative z-[1]"
              />
            </div>
          </div>
          <div class="p-[30px]">
            <h3 class="uppercase font-semibold text-secondary text-base">
              {{ element.name }}
            </h3>
            <p
              class="text-[14px] leading-[20px] text-white trackaing-[0.03rem]"
            >
              {{ element.description }}
            </p>
          </div>
        </div>
      </article>
    </div>
  </section>
</template>
<script setup>
import { ref } from "vue";
import SectionHeader from "@/components/UI/SectionHeader.vue";

const services = ref([
  {
    id: 1,
    icon: "https://img.icons8.com/ios-filled/100/daed1a/google-code.png",
    name: "Web Development",
    description:
      "Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatibus magnam corporis ullam dicta? Perspiciatis consequatur quis saepe, neque ea rem?",
  },
  {
    id: 2,
    icon: "https://img.icons8.com/external-vectorslab-glyph-vectorslab/100/daed1a/external-Technical-Writing-mobile-app-development-vectorslab-glyph-vectorslab.png",
    name: "Technical Writing",
    description:
      "Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatibus magnam corporis ullam dicta? Perspiciatis consequatur quis saepe, neque ea rem?",
  },
  {
    id: 3,
    icon: "https://img.icons8.com/ios-filled/100/daed1a/email-open.png",
    name: "Web Development",
    description:
      "Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatibus magnam corporis ullam dicta? Perspiciatis consequatur quis saepe, neque ea rem?",
  },
  {
    id: 4,
    icon: "https://img.icons8.com/ios-filled/100/daed1a/email-open.png",
    name: "Web Development",
    description:
      "Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatibus magnam corporis ullam dicta? Perspiciatis consequatur quis saepe, neque ea rem?",
  },
  {
    id: 5,
    icon: "https://img.icons8.com/ios-filled/100/daed1a/windows10-personalization.png",
    name: "Web Development",
    description:
      "Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatibus magnam corporis ullam dicta? Perspiciatis consequatur quis saepe, neque ea rem?",
  },
  {
    id: 6,
    icon: "https://img.icons8.com/ios-filled/100/daed1a/web-design.png",
    name: "Web Development",
    description:
      "Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatibus magnam corporis ullam dicta? Perspiciatis consequatur quis saepe, neque ea rem?",
  },
]);
</script>
