<script lang="ts" setup>
import { RouterLink } from 'vue-router'
</script>

<template>
  <div class="navbar">
    <div class="navbar-left">
      <RouterLink class="navbar-left-title" to="/">
        <img
          src="/images/mmorgat-2026-smaller.jpg"
          class="navbar-icon"
          alt="Photo of Mathieu"
          width="40"
          height="40"
        />
        <span class="navbar-left-title-name">Mathieu MORGAT</span>
      </RouterLink>
      <div class="navbar-elements">
        <RouterLink class="navbar-element" to="/">About</RouterLink>
        <RouterLink class="navbar-element" to="/background"
          >Background</RouterLink
        >
        <RouterLink class="navbar-element" to="/work">Work</RouterLink>
        <RouterLink class="navbar-element" to="/projects">Projects</RouterLink>
        <RouterLink class="navbar-element" to="/contact">Contact</RouterLink>
      </div>
    </div>
    <div class="navbar-right">
      <!-- WIP Language Selection -->
      <span class="navbar-link-icon">FR</span>
      <a
        class="navbar-link-icon"
        href="https://www.linkedin.com/in/mmorgat/"
        target="_blank"
      >
        <img src="/icons/linkedin.svg" alt="LinkedIn" width="24" height="24" />
      </a>
      <a
        class="navbar-link-icon"
        href="https://github.com/mmorgatDev"
        target="_blank"
      >
        <img src="/icons/github.svg" alt="GitHub" width="24" height="24" />
      </a>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 1.5rem;
  background-color: #333;
  color: #fff;

  .navbar-left {
    display: flex;
    align-items: center;

    .navbar-left-title {
      display: flex;
      align-items: center;
      text-decoration: none;
      color: #fff;
      gap: 0.75rem;
    }

    .navbar-icon {
      width: 40px;
      height: 40px;
      border-radius: 50%;
    }

    .navbar-left-title-name {
      font-size: 1.5rem;
      font-weight: bold;
      margin-right: 2rem;
      text-decoration: none;
    }

    .navbar-elements {
      display: flex;
      gap: 1.5rem;
    }

    .navbar-element {
      color: #fff;
      text-decoration: none;
      font-size: 1rem;
      font-weight: 500;
      cursor: pointer;

      &:hover {
        text-decoration: underline;
      }
    }

    .navbar-element.router-link-active {
      text-decoration: underline;
      font-weight: bold;
      cursor: default;
    }
  }

  .navbar-right {
    display: flex;
    align-items: center;
    gap: 1rem;

    .navbar-link-icon {
      display: flex;
      align-items: center;
      justify-content: center;
      background-color: white;
      padding: 0.5rem;
      border-radius: 50%;
      color: #333;
      text-decoration: none;
      font-size: 0.9rem;
      font-weight: bold;
      width: 24px;
      height: 24px;
      user-select: none;
    }
  }
}
</style>
