<script setup>
const props = defineProps({
  colorOptionOne: Object,
  colorOptionTwo: Object,
});
</script>

<template>
  <section aria-label="Select color:">
    <h3>Color:</h3>
    <hr />
    <article>
      <div>
        <button
          :style="{ backgroundColor: props.colorOptionOne.color }"></button>
        <p>{{ props.colorOptionOne.name }}</p>
      </div>
      <div>
        <button
          :style="{ backgroundColor: props.colorOptionTwo.color }"></button>
        <p>{{ props.colorOptionTwo.name }}</p>
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
  border: none;
  padding: 2rem;
  border-radius: 50%;
  outline: 1px solid gray;
  cursor: pointer;
  opacity: 0.5;
}

button:hover {
  outline: 1px solid white;
  transition: background 0.5s ease-in-out;
  opacity: 1;
}

hr {
  margin-top: 0.3rem;
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
