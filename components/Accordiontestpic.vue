<template>
  <v-row 
  justify="center"
  width="1600px">
    <v-expansion-panels accordion
    v-model="panel"
    light
    focusable
    Tile
    single
    >
      <!-- text="grey darken-4"
    color ="grey darken-4"
      light
      flat
      prominent -->
      <v-expansion-panel
      >
      <!-- color="grey darken-4"
      text="grey darken-4"
      light
      flat
      prominent
        v-for="(itemi) in 1"
        :key="i" -->
      <!-- The subject matter of the accordion -->
        <v-expansion-panel-header color ="grey lighten-5" text="grey darken-4">
         <v-expansion-panel-header-text color="grey darken-4"><h3>Tests Included </h3> </v-expansion-panel-header-text></v-expansion-panel-header>
        <v-expansion-panel-content color ="grey lighten-5"> 
        <!-- Due to a there being a long list of tests, heading styles and line changes were used to distinguish between the different tests -->
       <v-cols
       cols="12"
       sm="6"
       md="10"
       >
       <v-row>
       <prelim/> <diab/> <renal/> <liver/>
       </v-row>
       <v-row>
        <card/> <radio/> <spec/> <consul/>
        </v-row>
        </v-cols>

        </v-expansion-panel-content>
      </v-expansion-panel>
    </v-expansion-panels>
  </v-row>
</template>