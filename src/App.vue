<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
import footers from './components/footer.vue'
import Instagram from '@/components/icons/IconInstagram.vue'
import Telephone from '@/components/icons/IconTelephone.vue'
import Github from '@/components/icons/IconGithub.vue'
import Email from '@/components/icons/IconEmail.vue'

</script>

<template>
  <div class="bg-layer"></div>
  <header class="container">

      <nav class="text-center bg-light fixed-top">
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
  <RouterView />
  </header>
  <footer class="text-light">
    <footers>
      <template #footer-1>
        <h2 class="fw-bold">My Portfolio</h2>
      </template>
      <template #footer-2>
        <p>
          <Email/>
          andhikamardyanto34@gmail.com
        </p>
        <p>
          <Telephone/>
          081213517787
        </p>
        <p>
          <Github/>
          github/andhikamrdynto
        </p>
        <p>
          <Instagram/>
          @dhiikaa17
        </p>
      </template>
    </footers>
  </footer>

  
</template>

<style scoped>

footer {
  padding-block: 20px;
  background-color: #293462;
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
