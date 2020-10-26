<template>
    <v-fab-transition>

    <!-- I made a stick button component and edited it, and I added the component path in the 'nvf' page but I did not see the 
    component at all -->

    
        <v-btn
        :key="activeFab.icon"
        :color="activeFab.color"
        fab
        large
        dark
        bottom
        left
        class="v-btn--example"
      >
        <v-icon>{{ activeFab.icon }}</v-icon>
      </v-btn>
    </v-fab-transition>
</template>