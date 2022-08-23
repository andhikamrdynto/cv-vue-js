<script setup>
defineProps({
  msg: {
    type: String,
    required: true
  }
})
</script>

<template>
  <div class="greetings">
    <h1 class="text-dark fw-bold m-0">Andhika Mardyanto</h1>
    <h3>Frontend Developer</h3>
    <p class="text-center">
      Andhika is a student from Taruna
      Bhakti Vocational High School
      who is interested in IT fields
      such as programming

      <!-- <a target="_blank" href="https://vitejs.dev/">Vite</a> +
      <a target="_blank" href="https://vuejs.org/">Vue 3</a>. -->
    </p>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  top: -10px;
  font-family: sans-serif;
}

p {
  font-family: sans-serif;
  margin: auto;
  font-size: 12px;
  color: gray;
}

.greetings{
  margin-top: 3rem;
}
.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (max-width: 1000px) {
  .greetings h1{
    font-size: 2rem;
  }
}

@media (min-width: 1024px) {
  p{
    width: 400px;
  }
  .greetings h1,
  .greetings h3,
  .greetings p {
    text-align: center;
  }
}
</style>
