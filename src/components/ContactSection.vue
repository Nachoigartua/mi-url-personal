<template>
  <section class="section contact">
    <h2>Contacto</h2>
    <ul>
      <li><strong>Email:</strong> <a href="mailto:ignacioigartua15@gmail.com">ignacioigartua15@gmail.com</a></li>
      <li><strong>LinkedIn:</strong> <a href="https://www.linkedin.com/in/ignacio-igartua-088493324" target="_blank">Perfil profesional</a></li>
      <li><strong>Ubicación:</strong> Ciudadela, Buenos Aires, Argentina</li>
      <li><strong>Teléfono:</strong> +54 11 7058-6091</li>
    </ul>
  </section>
</template>

<script setup>
</script>

<style scoped lang="scss">
.section {
  margin-bottom: 3rem;
  h2 {
    color: #cc1c1c;
    margin-bottom: 1rem;
    border-bottom: 2px solid #cc1c1c;
    display: inline-block;
    padding-bottom: 0.2rem;
    animation: fadeIn 1s ease-in-out;
  }
  ul {
    list-style: none;
    padding: 0;
    li {
      margin-bottom: 0.5rem;
      line-height: 1.8;
      color: #444;
    }
  }
  a {
    color: #cc1c1c;
    text-decoration: none;
    font-weight: bold;
    transition: color 0.3s ease;
    &:hover {
      color: #a00;
      text-decoration: underline;
    }
  }
}
</style>
