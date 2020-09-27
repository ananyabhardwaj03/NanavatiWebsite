<template>
  <v-card>
    <v-toolbar
      color="#711843"
      dark
      flat
      prominent
    >
<!-- At first the search bar was leaving the screen but after adding the 'pt-5' class it came down the screen and was finally visible -->
  <VuetifyLogo/>

    <template class="ps-16">
  <v-cols cols="12"> <v-btn  class="md-8"  tile color="#711843" > 
  <strong class="white--text ">Book an Appointment</strong></v-btn></v-cols> 
  <v-cols cols="12"> <v-btn  class="md-8"  tile color="#711843" > 
  <strong class="white--text ">Log In</strong></v-btn></v-cols> 
  <v-cols cols="12"> <v-btn  class="md-8"  tile color="#711843" > 
  <strong class="white--text ">Register</strong></v-btn></v-cols> 
      </template>

<!-- The search bar did not have the icon at first but after adding the 'append-icon' and mdi-magnify icon it looked more like a search bar -->

      <v-text-field
        class="mx-4 pt-5"
        flat
        hide-details
        label="Search"
        append-icon="mdi-magnify"
      ></v-text-field>

<!-- I do not completely understand the meaning of v-slot:extention but still by using it I was able to 
distinguish between the two layers of buttons in the header -->

      <template  v-slot:extension>
        <v-tabs
          v-model="tabs"
          right
        >
          <v-tab
          >
            International Patients
          </v-tab>
           <v-tab
          >
            Doctors
          </v-tab>
           <v-tab
          >
            Outstation OPD 
          </v-tab>
          
          
        </v-tabs>
      </template>
    </v-toolbar>

   
  </v-card>
</template>

<script>
  export default {
    data () {
      return {
        tabs: null,
        text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.',
      }
    },
  }
</script>