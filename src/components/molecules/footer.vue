<script lang="ts" setup></script>

<template>
  <div class="footer">
    <div class="footer-left"></div>
    <p>Copyright &copy; 2026 Mathieu MORGAT</p>
    <div class="footer-right">
      <a
        class="footer-link-icon"
        href="https://www.linkedin.com/in/mmorgat/"
        target="_blank"
      >
        <img src="/icons/linkedin.svg" alt="LinkedIn" width="24" height="24" />
      </a>
      <a
        class="footer-link-icon"
        href="https://github.com/mmorgatDev"
        target="_blank"
      >
        <img src="/icons/github.svg" alt="GitHub" width="24" height="24" />
      </a>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.footer {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 2rem;
  background-color: #333;
  color: #fff;

  .footer-left,
  .footer-right {
    width: 20%;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 1rem;
  }

  .footer-link-icon {
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
</style>
