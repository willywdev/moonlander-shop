<script setup>
import { Icon } from "@iconify/vue";
</script>

<template>
  <header>
    <div aria-label="Socials">
      <a href="https://github.com/willywdev" target="_blank"
        ><Icon icon="mdi:github" width="42" aria-label="Github"
      /></a>
    </div>
    <div aria-label="Headline & Logo">
      <a href="/">
        <h1>Moonlander Shop</h1>
      </a>
    </div>

    <nav>
      <a href="/">
        <Icon icon="mdi:cart" width="42" aria-label="Cart" />
      </a>
    </nav>
  </header>
</template>

<style scoped>
header {
  background: rgb(47, 46, 46);
  height: 5rem;
  border-bottom: 1px solid rgb(80, 80, 80);
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 2rem 0 2rem;
  opacity: 0.7;
}
header:hover {
  opacity: 1;
}
</style>
