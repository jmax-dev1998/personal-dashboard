<template>
  <div class="bg-[#D4EBF8] dark:bg-[#080326] min-h-screen">
    <Navbar />
    <HeroSection />
    <Counter />
    <Services />
  </div>
</template>

<script setup>
import { defineAsyncComponent } from "vue";
const Navbar = defineAsyncComponent(() =>
  import("@/components/layouts/Navbar.vue")
);
const HeroSection = defineAsyncComponent(() =>
  import("@/components/layouts/HeroSection.vue")
);
const Counter = defineAsyncComponent(() =>
  import("@/components/layouts/Counter.vue")
);
const Services = defineAsyncComponent(() =>
  import("@/components/layouts/Services.vue")
);
</script>
