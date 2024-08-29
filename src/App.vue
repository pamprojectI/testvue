<script setup>
//import HelloWorld from './components/HelloWorld.vue'
//import TheWelcome from './components/TheWelcome.vue'
// import MyNev from './components/MyNev.vue'
import MyCard from './components/MyCard.vue'
// import items from './test.json'
import Menu from './components/Menu.vue'
import list from './list.json'
</script>

<template>
<div>
  <header>
    <Menu />
    <!-- <MyNev /> -->
    <!-- <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="512" /> 

    <div class="wrapper">
      <HelloWorld msg="You did it!" />
    </div> -->
  </header>

  <main>
    <h1>TheWelcome</h1>
    <div className="grid-container">
      <MyCard v-bind="list[0]" />
      <MyCard v-bind="list[1]" />
      <MyCard v-bind="list[2]" />
      
    </div>
    <!-- <TheWelcome /> -->
  </main>
</div>
</template>

<style scoped>
.grid-container {
  display: grid;
  grid-column-gap: 0.5rem;
  grid-row-gap: 0.5rem;
}
@media (min-width: 576px) {
  .grid-container { grid-template-columns: repeat(1, 1fr); }
}
@media (min-width: 992px) {
  .grid-container { grid-template-columns: repeat(3, 1fr); }
}

/* header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
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
} */
</style>
