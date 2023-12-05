<script setup>
import ColorSwitch from "@/components/ColorSwitch.vue";
</script>

<template>
  <main>
    <article>
      <h2>ZSA MOONLANDER</h2>
      <div class="image-container">
        <div class="radial-background"></div>
        <img src="../assets/heroes/hero_light.avif" alt="ZSA Moonlander" />
      </div>
    </article>
    <ColorSwitch />
  </main>
</template>

<style scoped>
main {
  height: 100vh;
}
.image-container {
  position: relative;
  width: 100%;
  height: 100%;
}
.radial-background {
  position: fixed;
  top: -10%;
  left: 0;
  width: 100%;
  height: 110%;
  background: radial-gradient(
    circle,
    rgba(255, 255, 255, 0.1) 0%,
    rgba(255, 255, 255, 0.09) 10%,
    rgba(255, 255, 255, 0.08) 20%,
    rgba(255, 255, 255, 0.07) 30%,
    rgba(255, 255, 255, 0.06) 40%,
    rgba(255, 255, 255, 0.05) 50%,
    rgba(255, 255, 255, 0.04) 60%,
    rgba(255, 255, 255, 0.03) 70%,
    rgba(255, 255, 255, 0.02) 80%,
    rgba(255, 255, 255, 0.01) 90%,
    rgba(255, 255, 255, 0) 100%
  );
  z-index: -5;
}
article {
  margin-top: 4rem;
  margin-bottom: 4rem;
  margin-left: 1rem;
  margin-right: 1rem;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
h2 {
  font-size: 4rem;
  background: #fafafa;
  color: #202020;
  text-align: center;
  margin-bottom: 2rem;
  padding: 0 4rem 0 3rem;
  box-shadow: rgba(50, 50, 93, 0.25) 0px 30px 60px -12px inset,
    rgba(0, 0, 0, 0.3) 0px 18px 36px -18px inset;
}
img {
  width: 100%;
  height: auto;
  padding: 2rem 0 2rem 0;
}
</style>
