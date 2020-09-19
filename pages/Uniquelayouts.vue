<template>
  <v-container class="grey lighten-5">
    <!-- Stack the columns on mobile by making one full-width and the other half-width -->
    <v-row>
      <v-col
        cols="22"
        md="12"
      >
        <v-card
          class="pa-2"
          outlined
          tile
        >
          .col-22 .col-md-12
        </v-card>
      </v-col>
      <v-col
        cols="8"
        md="6"
      >
        <v-card
          class="pa-4"
          outlined
          tile
        >
          .col-6 .col-md-4
        </v-card>
      </v-col>
    </v-row>

    <!-- Columns start at 50% wide on mobile and bump up to 33.3% wide on desktop -->
    <v-row>
      <v-col
        v-for="n in 3"
        :key="n"
        cols="6"
        md="4"
      >
        <v-card
          class="pa-2"
          outlined
          tile
        >
          Green
        </v-card>
      </v-col>
    </v-row>

    <!-- Columns are always 50% wide, on mobile and desktop -->
    <v-row>
      <v-col
        v-for="n in 2"
        :key="n"
        cols="6"
      >
        <v-card
          class="pa-2"
          outlined
          tile
        >
          .col-6
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>