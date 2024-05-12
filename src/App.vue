<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <header>
    
    <div class="wrapper">
      
    <h1>Ongoing Queues:</h1>
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div> 
  </header>

  <div class="container">

  <div class="first-column">
    <p>Now Serving OPD:</p>
  </div>

  <div class="second-column">
    <p>Total No. of Queues</p>
  </div>

  <div class="third-column">
    <div class="button-container">
      <!-- Buttons -->
      <button @click="back">Back</button>
      <button @click="next">Next</button>
      <button @click="edit">Edit</button>
    </div>
  </div>
</div>


<div class="container1">

<div class="first-column1">
  <p>Now Serving Check-up:</p>
</div>

<div class="second-column1">
  <p>Total No. of Queues</p>
</div>

<div class="third-column1">
  <div class="button-container1">
    <!-- Buttons -->
    <button @click="back">Back</button>
    <button @click="next">Next</button>
    <button @click="edit">Edit</button>
  </div>
</div>
</div>




  <RouterView />
</template>





<style scoped>

header .wrapper h1 {
  font-size: 20px;
  margin-left: 35px;
  margin-top: 15px;
  margin-bottom: 15px;
}


.container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-gap: 20px; 
  text-align: center;
  background-color: aliceblue;
  padding: 50px 0;
  margin: 0 35px 30px;
}

.first-column {
  
}

.second-column {
  border-left: 1.3px solid black;
  height: 100px;
}

.third-column {
  border-left: 1.3px solid black;
  height: 100px;
}

.button-container button {
  padding: 10px 20px;
  border: none;
  cursor: pointer;
  font-size: 12px;
  margin-right: 10px; /* Add a margin-right to create a gap between buttons */
}

.button-container button:last-child {
  margin-right: 0; /* Remove margin-right for the last button to avoid extra space */
}

.button-container button:nth-child(1) {
  background-color: blue;
  color: white;
}

.button-container button:nth-child(2) {
  background-color: blue;
  color: white;
}

.button-container button:nth-child(3) {
  background-color: gray;
  color: white;
}




/* second container start */

.container1 {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-gap: 20px; 
  text-align: center;
  background-color: aliceblue;
  padding: 50px 0;
  margin: 0 35px 30px;

}

.first-column1 {
  
}

.second-column1 {
  border-left: 1.3px solid black;
  height: 100px;
}

.third-column1 {
  border-left: 1.3px solid black;
  height: 100px;
}







/* 
header {
  line-height: 1.5;
  max-height: 100vh;
} */

/* .logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
} */
</style>


