<template>
  <div>
    <v-content>
    <!-- Breadcrumbs -->
      <Breadcrumbs/>
      <v-container>
      
        <v-row justify="Left-aligned"
        class="mb-10">
        
        <!-- Title Heading, Icon as well as description -->

<!-- Here we have the Women's Health Package Log0 (Illustrated Lady) -->
         <img
    src="wwp.jpg"
  > 

  <!-- Here the description of the Package Starts -->
         <v-col
         cols="12"
         md="10"
         sm="9"
         >
         <h1>Women's Health Package</h1>

         <!-- I wanted the description to move to the right of the icon but after playing around with it I is now below
         the icon and at first the <h4> was moving off the screen but after changing the order of the commands it ended up
         in the right place -->

         <h4> For The One Who Cares For Everyone:
        When she cares for everyone, how could we not care for her? Specially designed package for women.</h4>
        It's our quest to keep you in the pink of your health. Package designed for the ones who dedicate themselves to work but not health. A complete health check-up to determine any kind of risk posed by a hectic, stressful lifestyle.
         
</v-col>
        </v-row>

        <!-- The Accordion Component -->
        <Accordion/>

        <v-col
          cols="24"
         md="18"
         sm="12">
         
         </v-col>


      <v-row>
<!-- Here the Page is divided in multiple columns (4)  because I wanted to move the 'Book Now' buttom to the Right -->

<!-- Empty Columns -->
        <v-col
        justify="right"
        cols="12"
  sm="3"
  md="3">

        </v-col> 

<v-col
justify="right"
        cols="12"
  sm="3"
  md="3">

        </v-col>
        <v-col
        justify="right"
        cols="12"
  sm="3"
  md="3">

</v-col>
<!-- Empty Columns End Here -->

<!-- The 4th Column Starts Here -->
      <v-col
        justify="right"
        cols="12"
  sm="3"
  md="3">
  <Stickybutton/> <!-- The Sticky Button is not visible on the page for some reason -->

  <!-- Here we have the 'Book Now' Button -->
<Button/>

 </v-col>
<!-- The 4th Column Ends Here -->

</v-row>

      </v-container>
      <!-- End of Page Data -->
    </v-content>
  </div>
  
</template>

<script>
</script>

<style>
</style>
