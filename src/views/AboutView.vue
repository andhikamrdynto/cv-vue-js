<script setup>
import TheWelcome from '@/components/TheWelcome.vue'
</script>

<template>
  <div class="about container mb-5">
    <img alt="Vue logo" class="logo" src="public/photo/profile.jpeg"/>
    <div class="card">
      <div class="card-body">
        <main>
          <h1 class="text-center mt-2 fw-bold">My Skills</h1><hr>
          <TheWelcome/>
        </main>
      </div>
    </div>
  </div>
</template>

<style>

.logo {
  display: block;
  margin: 0 auto 2rem;
  border-radius: 50%;
  width: 240px;
  height: 240px;
  border: white 5px solid;
}


.about h1{
  font-family: sans-serif;
}

hr{
  border: 2px solid hsla(160, 100%, 37%, 1);
  border-radius: 10px;
  margin-bottom: 1.5rem;
}
@media (max-width: 1000px) {
  .about {
    margin-top: 2rem;
  }
}

@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    /* display: flex; */
    /* align-items: center; */
    margin-top: 2rem;
  }
}
</style>
