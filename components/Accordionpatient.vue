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
        <v-expansion-panel-header color ="grey lighten-5"><h3>Patient Stories</h3></v-expansion-panel-header>
        <v-expansion-panel-content color ="grey lighten-5">
          <p class="mt-15"><wa/><h4>Reena Tiwari, 49</h4></p>
          <p>"I am a very busy person, and I usually end up avoiding taking care of my health because I can't spare any extra time on that. But Nanavati's Health Packages were a gift and I was able to look after myself and in 
a very convenient and comfortable manner."</P>
<p><wb/><h4>Mirali Dixit, 38</h4></p>
<p>"The packages are designed for women in a very well thought-out manner. Taking numerous tests is usually bothersome, but this experience was so different than any other, and everything happened with ease."
</P>
<p><wc/><h4>Seema Sharma, 42</h4></p>
<p>"My experience at Nanavati Hospital was great! The doctors made me feel comfortable at every step and the package included all the important tests."
</P>
        </v-expansion-panel-content>
      </v-expansion-panel>
    </v-expansion-panels>
  </v-row>
</template>