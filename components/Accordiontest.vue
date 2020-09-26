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
        <v-expansion-panel-content color ="grey lighten-5"> <!-- Due to a there being a long list of tests, heading styles and line changes were used to distinguish between the different tests -->
         <P><H4>PRELIMINARY TESTS</h4></P><P>CBC with indices and platelet </P><P>
ESR </P><P>
Urine Routine </P><P>
Stool Routine</P>
  <P><H4>DIABETIC PROFILE</h4></P><P> Fasting Blood Sugar (F.B.S.) </P><P>
Post Prandial Blood Sugar (P.P.B.S) </P><P>
Glycosylated HB </P><P><h4>
RENAL TESTS </h4></P> S. Creatinine </P><P>
S. Calcium </P><P><h4>
LIVER TESTS</h4></p><p>
SGPT </p><p>
SGOT </p><p> <h4>
CARDIAC PROFILE </h4> </p><p>
Total Cholesterol </P><P>
S.Triglyceride</P><P>
HDL Cholesterol</P><P>
LDLC</P><P>
VLDL</P><P>
LDL/HDLC Ratio</P><P>
TC/HDLC Ratio</P><P>
ECG</P><P><h4>
RADIOLOGY </h4> </p><p>
Chest X-ray (PA View)</P><P>
USG (Abdomen and Pelvis)</P><P> <h4>
SPECIAL TESTS</h4> </p><p>
TSH</p><p>
Pap Smear</p><p>
Vitamin B12</p><p>
Vitamin D</p><p>
Mammography</p><p> <h4>
CONSULTATIONS </h4> </p><p>
Physician </p><p>
Dietician </p><p>
Gynaecologist </p>

        </v-expansion-panel-content>
      </v-expansion-panel>
    </v-expansion-panels>
  </v-row>
</template>