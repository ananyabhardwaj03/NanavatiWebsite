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
        <!-- The patient stories section has the pictures, basic information and the comments of the users -->
        <v-expansion-panel-header color ="grey lighten-5"><h3>About Your Doctors</h3></v-expansion-panel-header>
      </v-expansion-panel>
    </v-expansion-panels>
  </v-row>
</template>