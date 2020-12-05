<template>
<div class="container">
    <div id="news">
        <ComponenteNoticias></ComponenteNoticias>
    </div>
    
</div>
  
  
</template>

<script>
import ComponenteNoticias from "./components/ComponenteNoticias.vue";
export default {
  name: "App",
  components: {
    ComponenteNoticias,
  },
};
</script>

<style scoped>



</style>

