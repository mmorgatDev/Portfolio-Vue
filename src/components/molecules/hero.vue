<script lang="ts" setup>
const openPdf = () => {
  window.open('/docs/cv-mathieu-morgat-2026-vueJS.pdf', '_blank')
}
</script>

<template>
  <div class="hero">
    <img
      src="/images/mmorgat-2026.jpg"
      alt="Photo de Mathieu"
      width="200"
      height="200"
      class="hero-image"
    />
    <h1 class="hero-title">Mathieu MORGAT</h1>
    <p class="hero-paragraph">
      Bienvenue sur mon <span class="hero-highlight">portfolio web</span>!
      <br />Je suis un développeur
      <span class="hero-highlight">Frontend</span> spécialisé dans la conception
      et la réalisation d'interfaces de
      <span class="hero-highlight">WebApp</span> modernes, responsives et
      performantes.<br />Après cinq années d'études en développement
      <span class="hero-highlight">Fullstack</span>, dont trois en alternance,
      je recherche un poste à plein temps dans le développement Frontend avec
      <span class="hero-highlight">Vue.js</span>.
    </p>
    <div class="hero-links">
      <!-- Open CV PDF -->
      <button class="hero-link" @click="openPdf">Télécharger mon CV</button>
      <a
        href="https://www.linkedin.com/in/mmorgat/"
        target="_blank"
        class="hero-link"
        >LinkedIn</a
      >
    </div>
  </div>
</template>

<style lang="scss" scoped>
.hero {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  padding: 2rem;
  height: 100%;

  .hero-image {
    border-radius: 50%;
    margin-bottom: 1rem;
  }

  .hero-title {
    font-size: 2.5rem;
    margin-bottom: 1rem;
  }

  .hero-paragraph {
    font-size: 1.2rem;
    max-width: 70%;
    margin-bottom: 1.5rem;

    .hero-highlight {
      color: #007acc; /* Accent color */
      font-weight: bold;
    }
  }

  .hero-links {
    display: flex;
    gap: 1rem;

    .hero-link {
      padding: 0.5rem 1rem;
      background-color: #007acc; /* Accent color */
      color: #fff;
      text-decoration: none;
      border-radius: 4px;
      transition: background-color 0.3s;

      &:hover {
        background-color: #005f99; /* Darker accent on hover */
      }
    }
  }
}
</style>
