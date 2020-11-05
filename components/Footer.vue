<template>
   <v-footer 
      dark
      padless
      max-width="1980"
      class="grey darken-2 white--text text-left"
      >
      <!-- For this assignment, I had to work on my footer and to make it look more structured and similar to proper websites -->
      <v-container>
         <!-- In the Footer, I have 4 different columns, for 4 different headings -->
         <!-- The one and only row in the Footer starts here  -->
         <v-row>
            <!-- Column 1 starts here -->
            <v-col
               cols="12"
               sm="3"
               md="3"
               >
               <!-- In the first column I have Social media links for the users to get in touch with the website -->
               <v-spacer> </v-spacer>
               <H3> Connect With Us </h3>
               <v-divider></v-divider>
               <br>
               <!-- buttons of the different social media websites -->
               <v-btn
                  v-for="icon in icons"
                  :key="icon"
                  class="mx-2 white--text"
                  icon
                  >
                  <v-icon size="24px">{{ icon }}</v-icon>
               </v-btn>
            </v-col>
            <!-- Column 1 Ends Here -->
            <!-- Column 2 Starts Here -->
            <v-col
               cols="12"
               sm="3"
               md="3"
               >
               <v-spacer> </v-spacer>
               <H3> About Us </h3>
               <v-divider></v-divider>
               <br>
               <!-- 'v-spacers' are used here to align leave space wherever it is necessary -->
               <h4>
                  <font class="font-weight-regular">
                     About Nanavati Hospital 
                     <v-spacer> </v-spacer>
                     Community Services 
                     <v-spacer> </v-spacer>
                     Leadership  
                     <v-spacer> </v-spacer>
                     Newsroom  
                     <v-spacer> </v-spacer>
                     Awards   
                     <v-spacer> </v-spacer>
                     Sitemap  
                     <v-spacer> </v-spacer>
                     Privacy Policy 
                     <v-spacer> </v-spacer>
                     Terms of Use  
                     <v-spacer> </v-spacer>
                     Blogs
                  </font>
               </h4>
            </v-col>
            <!-- Column 2 Ends Here -->
            <!-- Column 3 Starts Here -->
            <v-col
               cols="12"
               sm="3"
               md="3"
               >
               <v-spacer> </v-spacer>
               <h3> Quick Links </h3>
               <v-divider></v-divider>
               <br>
               <h4>
                  <font class="font-weight-regular">
                     Patient Portal 
                     <v-spacer> </v-spacer>
                     STENT Pricing 
                     <v-spacer> </v-spacer>
                     TKR Implant Pricing 
                     <v-spacer> </v-spacer>
                     OPD Schedule 
                     <v-spacer> </v-spacer>
                     Transplant Data
                  </font>
               </h4>
            </v-col>
            <!-- Column 3 Ends Here -->
            <!-- Column 4 Start Here -->
            <v-col
               cols="12"
               sm="3"
               md="3"
               >
               <v-spacer> </v-spacer>
               <h3> Stay In Touch </h3>
               <v-divider></v-divider>
               <br>
               <h4>
                  <font class="font-weight-regular">
                     Dr. Balabhai Nanavati Hospital, 
                     <v-spacer> </v-spacer>
                     S.V. Road, Vile Parle (West), 
                     <v-spacer> </v-spacer>
                     Mumbai 400 056, India. <br> <br>
                     Tel: +91 22 6836 0000 
                     <v-spacer> </v-spacer>
                     Helpline: +91 22 2626 7500 <br> <br> 
                     Email:marketing@nanavatihospital.org  
                  </font>
                  <br> <br>
                  <!-- This column has images as well so they are added here, like this -->
                  <img
                     class="Radiant"
                     alt="Radiant"
                     src="Radiant.png"
                     > 
                  <img
                     class="Nabh"
                     alt="Nabh"
                     src="Nabh.png"
                     > 
               </h4>
            </v-col>
            <!-- Column 4 Ends Here -->
         </v-row>
         <!-- The Row Ends Here -->
      </v-container>
   </v-footer>
   <!-- The Footer Component Ends Here -->
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