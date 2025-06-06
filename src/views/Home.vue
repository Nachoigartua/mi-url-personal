<template>
  <section class="home">
    <IntroSection />
    <AboutSection />
    <ProjectsSection />
    <TechSection />
    <ContactSection />
  </section>
</template>

<script setup>
import IntroSection from '@/components/IntroSection.vue'
import AboutSection from '@/components/AboutSection.vue'
import ProjectsSection from '@/components/ProjectsSection.vue'
import TechSection from '@/components/TechSection.vue'
import ContactSection from '@/components/ContactSection.vue'
</script>

<style scoped lang="scss">
.home {
  padding: 2rem;
  max-width: 1000px;
  margin: 0 auto;
  font-family: 'Segoe UI', sans-serif;
  color: #222;
  background: linear-gradient(to bottom, #f9f9f9, #eaeaea);
  border-radius: 15px;
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
  animation: fadeIn 1.5s ease-in-out;

  @keyframes fadeIn {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
  }
}
</style>
