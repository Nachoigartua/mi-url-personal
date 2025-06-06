<template>
  <section class="section projects">
    <h2>Proyectos</h2>
    <div class="project-card" v-for="project in projects" :key="project.title">
      <h3>{{ project.title }}</h3>
      <p>{{ project.description }}</p>
      <a v-if="project.link" :href="project.link" target="_blank">Ver proyecto</a>
    </div>
  </section>
</template>

<script setup>
const projects = [
  {
    title: "Catálogo de APIs Web",
    description: "Proyecto front-end interactivo realizado con Vue.js y JavaScript para explorar, testear y documentar diversas APIs públicas. Incluye interfaz intuitiva, visualización de respuestas en tiempo real y gestión de tareas con Jira.",
    link: "https://github.com/patriciobaez/PNT2"
  },
  {
    title: "RojoFut11",
    description: "Plataforma de minijuegos diarios sobre el Club Atlético Independiente. Desarrollado con Vue.js, Vite y JavaScript. Diseño responsivo, componentes reutilizables y actualizaciones automáticas con JSON.",
    link: "https://nachoigartua.github.io/OnceRojo/#/minijuegos"
  },
  {
    title: "Sistema Académico Web",
    description: "Desarrollado con C# y .NET. Página web académica centrada en la gestión de pedidos de comida japonesa tipo sushi, con funcionalidades básicas y diseño profesional",
    link: null
  },
  {
    title: "App para Agencia de Lotería",
    description: "Desarrollé una aplicación financiera con .NET y Visual Basic, usando Windows Forms y una base de datos propia para gestionar cuentas, usuarios y operaciones administrativas.",
    link: null
  }
];
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
}
.project-card {
  border: 1px solid #ddd;
  padding: 1.5rem;
  border-radius: 10px;
  margin-bottom: 1.5rem;
  background: #fff;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  &:hover {
    transform: scale(1.05);
    box-shadow: 0 6px 15px rgba(0, 0, 0, 0.15);
  }
  h3 {
    margin: 0 0 0.5rem 0;
    color: #333;
    font-size: 1.5rem;
  }
  p {
    color: #555;
  }
}
</style>
