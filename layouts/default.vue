<template>

  <div class="layout">

    <div class="layout-bady">

      <logo></logo> 

      <background></background>

      <Nuxt />
        
      <info></info>

    </div>

  </div> 

</template>

<script> 

  import info from './../components/info.vue'
  import background from './../components/background.vue'
  import logo from './../components/logo.vue'
  
  export default {
    
    components: {
      info,
      background,
      logo,
    },
  }
  
</script>



<style>

  @import './../style/global.css';
  @import './../style/app.css';
  
</style>

















