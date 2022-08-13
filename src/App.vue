<template>
  <div id="app">
   <homePage></homePage>
  
  </div>
</template>

<script>
import homePage from "./views/homePage"
export default {
  components: {
    homePage
  }
}
</script>
<style scoped>
#app{
  height: 2000px;
}
</style>