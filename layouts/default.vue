<template>
  <!--Your App Starts Here -->
  <v-app id="inspire">
    
    
    <!-- Here we have the Header -->
    <Header/>  


    <p  class="mt-3 pl-3"> 
    Home  >  Specialty Health Packages  > Women's Health Package
</p>


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