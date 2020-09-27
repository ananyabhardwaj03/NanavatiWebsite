<template>
  <div>
    <v-content>
    <!-- Breadcrumbs -->
      <Breadcrumbs/>
      <v-container>
        <v-row justify="Left-aligned">
        
        <!-- Title Heading, Icon as well as description -->

         <wwp/> 
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
        <Accordiontestpic/>
        <Accordiondoc/>
        <Accordionpatient/>

        <v-col
        justify="right"
        cols="12"
        sm="8"
        md="10">
        <Button/>
        </v-col>


      </v-container>
    </v-content>
  </div>
  
</template>

<script>
</script>

<style>
</style>
