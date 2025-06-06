<template>
  <div class="intro">
    <img src="@/assets/Ignacio.jpg" alt="Ignacio Igartua" class="profile-img" />
    <div class="intro-text">
      <h1>Ignacio Igartua</h1>
      <p class="tagline">Desarrollador web en formación, apasionado por crear soluciones tecnológicas con impacto real.</p>
    </div>
  </div>
</template>

<script setup>
</script>

<style scoped lang="scss">
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
</style>
