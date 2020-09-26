<template>
  <!--Your App Starts Here -->
  <v-app id="inspire">
    
    
    <!-- -->
    <Header/>  
   <nvlogo/>

    <!-- Body -->
    <v-content light>
      <nuxt /> 
    </v-content>
    
    <!--  -->   
    <Footer/>    

  </v-app>
</template>

<script>
export default {}
</script>

<style> 
  .white--text {
    border: 1px solid;
  }

   #inspire {
    background-color: white;
    color: black;
  }
</style>