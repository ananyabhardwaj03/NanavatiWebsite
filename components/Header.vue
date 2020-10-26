<template>
  <v-card>

<!-- My old header component was not up to par, so here I made a new footer component to work on -->

    <v-toolbar
      color="#711843"
      dark
      flat
    >

    <!-- This Header component is divided into 2 Rows -->

    <!-- Row 1 Starts Here -->
    <v-row>

  <!-- Row 1 has 3 Columns
  Column 1 - Website Logo
  Column 2 - Login/Registration Buttons
  Column 3 - Search Bar -->

  <!-- Column 1 (Row 1) Starts Here -->
  <v-col
  col=12
  sm=5
  md=5>

  <!-- The website logo is inserted here -->
      <img
    class="VuetifyLogo"
    alt="Vuetify Logo"
    src="nvlogore.jpg"
  >

</v-col>
<!-- Column 1 (Row 1)  Ends Here -->

<!-- Column 2 (Row 1) Starts Here -->
  <v-col
col=12
sm=3
md=3>
 
 <!-- Here we have the 3 buttons of row 1 -->
           <div class="my-2 mt-10">

           <v-btn
              small
              color="#711843"
              dark
            >
              Book An Appointment
            </v-btn>

            <v-btn
              small
              color="#711843"
              dark
            >
              Log In
            </v-btn>
           
            <v-btn
              small
              color="#711843"
              dark
            >
              Register
            </v-btn>
          </div>

</v-col>
<!-- Column 2 (Row 1) Ends Here -->

<!-- Column 3 (Row 1) Starts Here -->
<v-col
col=12
sm=4
md=4>
      <v-spacer></v-spacer>
<!-- At first 1 had problems with the toolbar as it was originally taking up too much space,
but after adding the columns, margins, paddings, it shrunk and fir the website better -->
      <v-text-field
        class="ps-16 mt-8"
        flat
        hide-details
        label="Search"
        append-icon="mdi-magnify"
      ></v-text-field>

</v-col>
<!-- Column 3 (Row 1) Ends Here -->


      </v-row>
      <!-- Row 1 Ends Here -->


<!-- I do not fully grasp the function of slot:extension, though I have used it in my code -->
      <template v-slot:extension>

<!-- The Second Row of my website is divided into 2 columns, the first one doesn't have any data and was made mainly for the column 2
data, as it fits better, and on the right side of the page in the second column-->


      <!-- Row 2 of the Header starts here -->
      <v-row>

<!-- Column 1 (Row 2) Starts Here -->
<v-col
col=12
sm=7
md=7>
</v-col>
<!-- Column 1 (Row 2) Ends Here -->

<!-- Column 2 (Row 2) Starts Here -->
<v-col
col=12
sm=5
md=5>

<!-- This col has 3 Buttons that can be found on the Header -->
               <div class="my-2">
            <v-btn
              color="#711843"
              dark
            >
              International Patients
            </v-btn>

            <v-btn
              color="#711843"
              dark
            >
              Doctors
            </v-btn>

            <v-btn
              color="#711843"
              dark
            >
              Outstation OPD
            </v-btn>

          </div>
      </v-col>
<!-- Column 2 (Row 2) Ends Here  -->

      </v-row>
      <!-- Row 2 Ends Here -->


      </template>
  </v-toolbar>
 <!-- The Header Component Ends Here -->


    <v-tabs-items v-model="tab">
      <v-tab-item
        v-for="item in items"
        :key="item"
      >
        <v-card flat>
          <v-card-text v-text="text"></v-card-text>
        </v-card>
      </v-tab-item>
    </v-tabs-items>
  </v-card>
</template>