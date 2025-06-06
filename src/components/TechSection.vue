<template>
  <section class="section tech">
    <h2>Tecnologías y herramientas</h2>
    <ul>
      <li><strong>Lenguajes:</strong> Java, C#, JavaScript</li>
      <li><strong>Frontend:</strong> Vue.js, Vite, Bootstrap, jQuery, HTML, CSS</li>
      <li><strong>Backend / BD:</strong> ASP.NET MVC, SQL Server</li>
      <li><strong>Herramientas:</strong> Git, GitHub, Visual Studio, Figma, Bizagi</li>
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
}
</style>
