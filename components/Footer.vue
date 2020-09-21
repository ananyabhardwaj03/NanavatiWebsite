<template>
  <v-footer
    dark
    padless
    max-width="1980"
  >
  <!-- The footer has to cover the whole page, at first it was only occupying a section of the screen but then after 
  making changes is the max-width as well as adding more text it finally fit the width of the screen -->
    <v-card
      flat
      tile
      class="grey darken-1 white--text text-center"
    >
    <v-card-text class="white--text pt-5">
        Connect With Us
<v-btn
          v-for="icon in icons"
          :key="icon"
          class="mx-4 white--text"
          icon
        >
          <v-icon size="24px">{{ icon }}</v-icon>
        </v-btn>
      </v-card-text>
<!-- At first the text was all fitting in one line and not in different paragraphs/sections but after playing around I then made different
cards and added heading levels, as well as dividers to be able to differentiate between the sections -->
      <v-card-text>
        <h3>About Us:</h3>
       <h4> About Nanavati Hospital      Community Services      Leadership      Newsroom      Awards      Sitemap      Privacy Policy      Terms of Use      Blogs</h4>
      </v-card-text>

     <v-divider></v-divider>

       <v-card-text>
      <h3>Quick Links:</h3>
      <h4>Patient Portal
STENT Pricing
TKR Implant Pricing
OPD Schedule
Transplant Data</h4>
      </v-card-text>

     <v-divider></v-divider>

<!-- Different cards  have different types of information -->

      <v-card-text class="white--text pt-5">
       <h3>Stay in Touch</h3>
       Dr. Balabhai Nanavati Hospital, 
S.V. Road, Vile Parle (West), 
Mumbai 400 056, India.
Tel:+91 22 6836 0000
24 Hrs helpline: +91 22 2626 7500
Email:marketing@nanavatihospital.org
Managed By: Radiant (Life Car Private Limited)
NABH and NABL Accredited
      </v-card-text>

      <v-divider></v-divider>

      <v-card-text class="white--text">
        {{ new Date().getFullYear() }} — <strong>Nanavati Specialty Hospital</strong>
      </v-card-text>
    </v-card>
  </v-footer>
</template>

<script>
  export default {
    data: () => ({
      icons: [
        'mdi-facebook',
        'mdi-twitter',
        'mdi-linkedin',
        'mdi-instagram',
      ],
    }),
  }
</script>