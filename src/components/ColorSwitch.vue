<script setup></script>
<template>
  <section aria-label="Select color:">
    <h3>Color:</h3>
    <hr />
    <article>
      <div>
        <button></button>
        <p>Color 1</p>
      </div>
      <div>
        <button></button>
        <p>Color 2</p>
      </div>
    </article>
  </section>
</template>
<style scoped>
section {
  display: flex;
  flex-direction: column;
  align-items: center;
  font-size: x-large;
}

article {
  display: flex;
  gap: 1rem;
  margin-top: 1rem;
}

button {
  background: rgba(255, 255, 255, 0.1);
  border: none;
  padding: 2rem;
  border-radius: 50%;
  outline: 1px solid gray;
  cursor: pointer;
}

button:hover {
  background: rgba(255, 255, 255, 0.2);
  outline: 1px solid white;
  transition: background 0.5s ease-in-out;
}

hr {
  margin-top: 1rem;
  width: 75%;
}

div {
  display: flex;
  flex-direction: column;
  align-items: center;
  font-size: medium;
  gap: 0.5rem;
}
</style>
