<template>
  <section class="home">
    <div class="intro">
      <img src="@/assets/Ignacio.jpg" alt="Ignacio Igartua" class="profile-img" />
      <div class="intro-text">
        <h1>Ignacio Igartua</h1>
        <p class="tagline">Desarrollador web en formación, apasionado por crear soluciones tecnológicas con impacto real.</p>
      </div>
    </div>

    <section class="section about">
      <h2>Sobre mí</h2>
      <p>
        Estudiante de la Tecnicatura en Análisis de Sistemas en ORT Almagro. 
        Tengo experiencia en el desarrollo de software, diseño web y soporte técnico. 
        Disfruto trabajar en proyectos que combinan creatividad, eficiencia e innovación. 
        Me apasiona el desarrollo de videojuegos, el diseño digital y el aprendizaje continuo.
      </p>
    </section>

    <section class="section projects">
      <h2>Proyectos</h2>
      <div class="project-card" v-for="project in projects" :key="project.title">
        <h3>{{ project.title }}</h3>
        <p>{{ project.description }}</p>
        <a v-if="project.link" :href="project.link" target="_blank">Ver proyecto</a>
      </div>
    </section>

    <section class="section tech">
      <h2>Tecnologías y herramientas</h2>
      <ul>
        <li><strong>Lenguajes:</strong> Java, C#, JavaScript</li>
        <li><strong>Frontend:</strong> Vue.js, Vite, Bootstrap, jQuery, HTML, CSS</li>
        <li><strong>Backend / BD:</strong> ASP.NET MVC, SQL Server</li>
        <li><strong>Herramientas:</strong> Git, GitHub, Visual Studio, Figma, Bizagi</li>
      </ul>
    </section>

    <section class="section contact">
      <h2>Contacto</h2>
      <ul>
        <li><strong>Email:</strong> <a href="mailto:ignacioigartua15@gmail.com">ignacioigartua15@gmail.com</a></li>
        <li><strong>LinkedIn:</strong> <a href="https://www.linkedin.com/in/ignacio-igartua-088493324" target="_blank">Perfil profesional</a></li>
        <li><strong>Ubicación:</strong> Ciudadela, Buenos Aires, Argentina</li>
        <li><strong>Teléfono:</strong> +54 11 7058-6091</li>
      </ul>
    </section>
  </section>
</template>

<script setup>
const projects = [
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
  },
  {
    title: "Sistema de Gestión de Pagos",
    description: "Aplicación de escritorio en Visual Basic .NET para supermercados. Manejo de deudas y pagos con interfaz clara.",
    link: null
  }
];
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

  .intro {
    display: flex;
    align-items: center;
    gap: 1.5rem;
    margin-bottom: 3rem;
    animation: slideIn 1s ease-in-out;

    .profile-img {
      width: 120px;
      height: 120px;
      object-fit: cover;
      border-radius: 100%;
      border: 3px solid #cc1c1c;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
      transition: transform 0.3s ease;

      &:hover {
        transform: scale(1.1);
      }
    }

    .intro-text {
      h1 {
        font-size: 2.5rem;
        margin: 0;
        color: #333;
        text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.1);
      }

      .tagline {
        font-size: 1.2rem;
        color: #555;
        font-style: italic;
      }
    }
  }

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

    p, li {
      line-height: 1.8;
      color: #444;
    }

    ul {
      list-style: none;
      padding: 0;

      li {
        margin-bottom: 0.5rem;
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

  @keyframes fadeIn {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
  }

  @keyframes slideIn {
    from { opacity: 0; transform: translateX(-50px); }
    to { opacity: 1; transform: translateX(0); }
  }
}
</style>
