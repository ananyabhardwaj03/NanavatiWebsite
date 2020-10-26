<template>
  <div>

<!-- Here I have attempted to put the breadcrumbs -->

    <v-breadcrumbs :items="items">
      <template v-slot:divider>
      Home
        <v-icon>mdi-forward</v-icon>
        Specialty Health Packages
        <v-icon>mdi-forward</v-icon>
        Well Women's Package
      </template>
    </v-breadcrumbs>

  </div>
</template>