<template>
  <v-row 
  justify="center"
  >

    <v-expansion-panels accordion
    v-model="panel"
    light
    focusable
    Tile
    single>

    <!-- For this assignment I had to find a way to input data dynamically in one component, i.e. Have only one accordion component
    instead of three. After a few trials and errors, I realized I could put the <v-expansion-panel> bracket 
    multiple times inside the <v-expansion-panels> umbrella component-->

<!-- There are 3 Accordions here
Accordion 1 - Tests Included
Accordion 2 - About Your Doctors
Accordion 3 - Patient Stories -->


<!-- Accordion 1 Starts Here -->
    <v-expansion-panel
    v-for="(item,i) in "
    :key="i">

      <v-expansion-panel-header color ="grey lighten-5" text="grey darken-4">
      <v-expansion-panel-header-text color="grey darken-4"><h3>Tests Included </h3> </v-expansion-panel-header-text></v-expansion-panel-header>
      <v-expansion-panel-content color ="grey lighten-5"> 
<!-- Due to a there being a long list of tests, heading styles and line changes were used to distinguish between the different tests -->
       

<!-- In this accordion I have multiple cards containing all the different test names and information  -->

<!-- Inside this accordion I have 8 tests, which are divided in 2 Rows, and each row has 4 Columns -->

<!-- Row 1 (R1) Starts Here -->
       <v-row
       class="mt-6" 
       >

<!-- Test 1, Column 1 (R1) -->
      <v-cols
      class="ml-6 mb-6" 
       cols="8"
       sm="2"
       md="2"
       > <v-card> <img
    class="prelim"
    alt="prelim"
    src="prelim.jpg"
  > </v-card> </v-cols> <V-spacer> </v-spacer>

<!-- Test 2, Column 2 , (R1) -->
       <v-cols
       cols="8"
       sm="4"
       md="4"
       ><v-card> <img
    class="diab"
    alt="diab"
    src="diab.jpg"
  > </v-card> </v-cols> <V-spacer> </v-spacer>
        
<!-- Test 3, Column 3 (R1) -->
        <v-cols
       cols="8"
       sm="6"
       md="6"
       > <v-card> <img
    class="renal"
    alt="renal"
    src="renal.jpg"
  > </v-card> </v-cols> <V-spacer> </v-spacer>

<!-- Test 4, Column 4, (R1) -->
       <v-cols
       class="mr-6" 
       cols="8"
       sm="8"
       md="8"
       > <v-card> <img
    class="liver"
    alt="liver"
    src="liver.jpg"
  > </v-card> </v-cols>

       </v-row>
       <!-- Row 1 Ends Here -->

       <!-- Row 2 (R2) Starts Here -->
       <v-row
       class="mb-6" >

<!-- Test 5, Column 1 (R2) -->
        <v-cols
        class="ml-6" 
       cols="8"
       sm="2"
       md="2"
       > <v-card>  <img
    class="card2"
    alt="card"
    src="card.jpg"
  >  </v-card> </v-cols> <V-spacer> </v-spacer>
      
      <!-- Test 6, Column 2 (R2) -->
       <v-cols
       cols="8"
       sm="2"
       md="2"
       ><v-card> <img
    class="radio"
    alt="radio"
    src="radio.jpg"
  >  </v-card> </v-cols> <V-spacer> </v-spacer>
       
       <!-- Test 7, Column 3 (R2) -->
        <v-cols
       cols="8"
       sm="2"
       md="2"
       > <v-card> <img
    class="spec"
    alt="spec"
    src="spec.jpg"
  > </v-card> </v-cols> <V-spacer> </v-spacer>
       
       <!-- Test 8, Column 4 (R2) -->
        <v-cols
        class="mr-6" 
       cols="8"
       sm="2"
       md="2"
       > <v-card> <img
    class="consul"
    alt="consul"
    src="consul.jpg"
  > </v-card> </v-cols>

        </v-row>
        <!-- Row 2 Ends Here -->
        

        </v-expansion-panel-content>
      </v-expansion-panel>
<!-- Accordion 1 Ends Here -->

<!-- Accordion 2 Starts Here  -->

      <v-expansion-panel
        v-for="(item,i) in 1"
        :key="i"
      >
        <v-expansion-panel-header color ="grey lighten-5"><h3>About Your Doctors</h3></v-expansion-panel-header>
        <v-expansion-panel-content>

<!-- Inside this Accordion, we have 3 cards, with 3 doctors' information on it-->


<!-- All 3 cards are in one row, in 3 different columns, and have padding and margin applied on them to fit inside the card properly -->

<!-- Accordion 2 'Row' Starts Here -->
<v-row class="mt-6 mb-1 ml-6 mr-6">

<!-- Card 1 (Doctor 1) Starts Here -->
      <v-col>
      
       <v-card
       class= "pl-3 pr-3" 
       ><p class= "pt-4" >
          <img
    class="d1"
    alt="d1"
    src="d1.jpg"
  > <h4>Dr. Gayatri Deshpande</h4></p> 
        <h5>  Sr Consultant - Obstetrics and Gynaecology </h5>
 <p class= "pb-4" >
Department
Gynaecology and Obstetrics</P> </v-card>
</v-col>
<!-- Card 1 (Doctor 1) Ends Here -->

<!-- Card 2 (Doctor 2) Starts here-->
<v-col>
<v-card  class= "pl-3 pr-3" > <p  class= "pt-4" ><img
    class="d2"
    alt="d2"
    src="d2.jpg"
  >><h4>Dr. Preeti D. Galvankar</h4></p>
<h5> Consultant - Obstetrics and Gynaecology </h5>
<p  class= "pb-4"  > 
Department
Gynaecology and Obstetrics
</P> </v-card>
</v-col>
<!-- Card 2 (Doctor 2) Ends Here -->

<!-- Card 3 (Doctor 3) Starts Here -->
<v-col>
<v-card  class= "pl-3 pr-3"  > <p  class= "pt-4"  ><img
    class="d3"
    alt="d3"
    src="d3.jpg"
  ><h4>Dr. Madhuri V. Joshi</h4></p>
<h5> Consultant - Gynaecology and Obstetrics </h5>
<p  class= "pb-4"  > 
Department
Gynaecology and Obstetrics
</P> </v-card>
</v-col>
<!-- Card 3 (Doctor 3) Ends Here -->

</v-row>
<!-- Accordion 2 'Row' Ends Here-->

        </v-expansion-panel-content>
      </v-expansion-panel>
      <!-- Accordion 2 Ends Here -->



<!-- Accordion 3 Starts Here -->
      <v-expansion-panel
        v-for="(item,i) in 1"
        :key="i"
      >
<!-- Inside this Accordion we have 'Patient Stories', and we have 3 diifferent patients on 3 different (horizontal) cards here  -->
        <v-expansion-panel-header color ="grey lighten-5"><h3>Patient Stories</h3></v-expansion-panel-header>
        <v-expansion-panel-content color ="grey lighten-5" class="mt-10 mb-10">

        <!-- Card 1 (Patient 1) Starts Here -->
          <v-card  class="pt-4 pb-3 pl-4 pr-4">  <v-row> <v-col col=12 md=2 sm=2>  <p >
          <img
    class="wa"
    alt="wa"
    src="wa.jpg"
  >  <h4>Reena Tiwari, 49</h4></p> </v-col> <v-col col=12 md=10 sm=10>
          <p class="pl-4 pr-4 mt-14">"I am a very busy person, and I usually end up avoiding taking care of my health because I can't spare any extra time on that. But Nanavati's Health Packages were a gift and I was able to look after myself and in 
a very convenient and comfortable manner." </p> 
</v-col> </v-row>
</v-card>
<!-- Card 1 (Patient 1)  Ends Here -->

<!-- Card 2 (Patient 2)  Starts Here-->
<v-card  class="pt-4 pb-3 pl-4 pr-4">
<v-row> <v-col col=12 md=2 sm=2>  
<p><img
    class="wb"
    alt="wb"
    src="wb.jpg"
  ><h4>Mirali Dixit, 38</h4></p> </v-col> <v-col col=12 md=10 sm=10>
<p class="pl-4 pr-4 mt-14">"The packages are designed for women in a very well thought-out manner. Taking numerous tests is usually bothersome, but this experience was so different than any other, and everything happened with ease."
</p>
 </v-col> </v-row>
 </v-card>
<!-- Card 2 (Patient 2) Ends Here -->

<!-- Card 3 (Patient 3) Starts Here -->
 <v-card class="pt-4 pb-3 pl-4 pr-4">
<v-row> <v-col col=12 md=2 sm=2>
<p><img
    class="wcc"
    alt="wcc"
    src="wcc.png"
  ><h4>Seema Sharma, 42</h4></p> </v-col> <v-col col=12 md=10 sm=10>
<p class="pl-4 pr-4 mt-14">"My experience at Nanavati Hospital was great! The doctors made me feel comfortable at every step and the package included all the important tests."
</p> 
</v-col> </v-row>
</v-card> 
<!-- Card 3 (Patient 3) Ends Here -->

        </v-expansion-panel-content>

      </v-expansion-panel>
<!-- Accordion 3 Ends Here -->


    </v-expansion-panels>
    <!-- The Accordion Component Ends Here -->
  </v-row>
</template>

