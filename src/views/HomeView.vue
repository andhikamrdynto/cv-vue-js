<script setup>
  import DisplayGrid from '@/components/DisplayGrid.vue'
  import HelloWorld from '@/components/HelloWorld.vue'
</script>

<template>
  <div class="home container">
    <img alt="Vue logo" class="logo" src="public/photo/profile.jpeg"/>

      <HelloWorld msg="You did it!" />
    <main>
      <h1 class="text-center fw-bold mt-5 mb-5">My Projects</h1>
      <DisplayGrid class="mb-5 reverse">
        <template #grid-1>
          <img src="public/photo/landing.png" alt="">
          <img src="public/photo/landing-2.png" alt="">
        </template>
        <template #grid-2>
          <h2>Landing Page with HTML, CSS, Bootstrap</h2>
        </template>
      </DisplayGrid>
      <DisplayGrid class="mb-5 column">
        <template #grid-1>
          <h2>Duplicate Valorant with HTML, CSS, JavaScript</h2>
        </template>
        <template #grid-2>
          <img src="public/photo/valorant-1.png" alt="">
          <img src="public/photo/valorant-2.png" alt="">
        </template>
      </DisplayGrid>
    </main>
  </div>
</template>

<style scoped>
  .home h1,
  h2 {
    font-family: sans-serif;
  }

  img {
    border: 0.5px solid gray;
    border-radius: 5px;
    width: 400px;
    height: 200px;
  }

  img:nth-child(2) {
    margin-left: 3rem;
    margin-top: -6rem;
  }

  footer {
    padding-block: 20px;
    background-color: #293462;
  }

  @media (min-width: 600px) and (max-width: 1000px) {
    .reverse{
      display: flex;
      flex-direction: column-reverse;
    }
  }

  @media (max-width: 600px) {
    img {
      width: 300px;
      height: 150px;
    }

    .home h2{
      font-size: 18px;
    }

    .reverse{
      display: flex;
      flex-direction: column-reverse;
    }

    .column{
      display: flex;
      flex-direction: column;
    }
  }

  .bg-layer{
  background-color: #293462;
  height: 280px;
  margin-bottom: -180px;
}

header {
  line-height: 1.5;
  min-height: 90vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
  border-radius: 50%;
  width: 240px;
  height: 240px;
  border: white 5px solid;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  /* margin-top: 2rem; */
  padding: 10px 0;
  height: 50px;
}

nav a::before{
  content: '';
  width: 0;
}

nav a:hover::before{
  content: '';
  background-color: #293462;
  width: 50px;
  height: 2px;
  position: absolute;
  bottom: 0;
  transition: ease-in 0.3s;
}

nav a.router-link-exact-active {
  color: #293462;
}

nav a {
  position: relative;
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (max-width: 600px) {
  header {
    min-height: 78vh;
  }
  .logo{
    width: 180px;
    border: 3px solid white;
    height: 180px;
  }
  nav{
    padding: 15px 0;
  }

  .bg-layer{
  height: 280px;
  margin-bottom: -130px;
}
}

@media (min-width: 600px) and (max-width: 834px){
  header {
    min-height: 80vh;
  }
}

@media (min-width: 884px) and (max-width: 1000px){
  header {
    min-height: 70vh;
  }
}


@media (min-width: 1024px) {

  .logo {
    margin: auto;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
    height: 80vh;
  }

  nav {
    text-align: left;
    font-size: 1rem;

    /* padding: 1rem 0; */
    /* margin-top: 1rem; */
  }
}
</style>