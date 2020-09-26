<template>
  <v-container class="grey lighten-5">
    <v-row
      class="mb-6"
      no-gutters
    >
      <v-col
        v-for="n in 4"
        :key="n"
        sm="8"
        md="4"

      >
        <v-card
          class="pa-2"
          tile
          outlined
        >
          col
        </v-card>
        <v-card
          class="pa-2"
          tile
          outlined
        >
          col
        </v-card>
        <v-card
          class="pa-2"
          tile
          outlined
        >
          col
        </v-card>
      </v-col>
    </v-row>

    <v-row no-gutters>
      <v-col
        v-for="n in 2"
        :key="n"
        :cols="n === 1 ? 11 : 4"
      >
        <v-card
          class="pa-2"
          tile
          outlined
        >
          col-{{ n === 2 ? 6 : 5 }}
        </v-card>
        <v-card
          class="pa-2"
          tile
          outlined
        >
          col-{{ n === 1 ? 5 : 5 }}
        </v-card>
        <v-card
          class="pa-2"
          tile
          outlined
        >
          col-{{ n === 1 ? 4 : 5 }}
        </v-card>
      </v-col>
    </v-row>
  </v-container>

 
</template>