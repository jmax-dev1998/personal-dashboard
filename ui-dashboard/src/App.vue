<template>
  <div class="bg-[#B6FFFA] dark:bg-[#211951] min-h-screen">
    <Suspense>
      <template #default>
        <div>
          <Navbar />
          <HeroSection />
          <Counter />
          <Services />
          <Skills />
          <Whyme />
          <Projects />
          <Contact />
          <Footer />
          <BackToTop />
        </div>
      </template>

      <template #fallback>
        <div class="flex justify-center items-center min-h-screen">
          <LoadingSpinner />
        </div>
      </template>
    </Suspense>
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
const Skills = defineAsyncComponent(() =>
  import("@/components/layouts/Skills.vue")
);
const Whyme = defineAsyncComponent(() =>
  import("@/components/layouts/Whyme.vue")
);
const Projects = defineAsyncComponent(() =>
  import("@/components/layouts/Projects.vue")
);
const Contact = defineAsyncComponent(() =>
  import("@/components/layouts/Contact.vue")
);
const Footer = defineAsyncComponent(() =>
  import("@/components/layouts/Footer.vue")
);
const BackToTop = defineAsyncComponent(() =>
  import("@/components/layouts/BackToTop.vue")
);
const LoadingSpinner = defineAsyncComponent(() =>
  import("@/components/layouts/LoadingSpinner.vue")
);
</script>

<style>
* {
  scrollbar-width: thin;
  scrollbar-color: #111827 #f1f1f1;
}
</style>
