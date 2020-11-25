<template>
  <div id="app">
    <!-- Set name or it defaults to '/' in router.js -->
    <router-view/>
  </div>
</template>

<script>
export default {
  name: "app"
};
</script>

<!-- global styles -->
<style>
@import url('https://fonts.googleapis.com/css2?family=Varela&display=swap&family=Montserrat:wght@200;400;600;700;800&display=swap');

* {
  box-sizing: border-box;
}

body {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background-color: #FFFFFF;
  margin: 0;
}

.success-message {
  color: green;
  margin: auto;
}

.error-message {
  color: red;
  margin: auto;
}
</style>