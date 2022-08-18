<template>
  <div class="app">
    <Navbar/>
    <h1>Hello</h1>
  </div>
</template>

<script>
import Navbar from '@/components/UI/Navbar.vue';

export default {
  name: 'App',
  components: {
    Navbar,
  }
}
</script>

<style lang="scss">
* {
  box-sizing: border-box;
}

ul {
  margin: 0;
  padding: 0;
  list-style: none;
}

h1,
h2,
h3,
p {
  margin: 0;
}

a {
  text-decoration: none;
}

.container {
  max-width: 1440px;
  margin: auto;
}

</style>
