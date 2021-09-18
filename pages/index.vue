<template>
<div>
  <v-sheet min-height="600">
    <v-row class="jumbo" no-gutters style="height: 1000px" tag="section">
      <v-col style="z-index: 1; isolation: isolate">
        <v-sheet class="pa-16 transparent"
          ><h1 class="font-weight-bold text-h1 mt-12">Expertos en impermeabilizaciones</h1>
          <h2 class="font-weight-light my-3">Con más de 20 años de experiencia</h2>
          <p>
            <PrimaryButton />
          </p></v-sheet
        >
      </v-col>
      <v-spacer></v-spacer>
    </v-row>
  </v-sheet>
  <v-container>
        <v-row>
          <v-col
            v-for="n in 6"
            :key="n"
            lg="3"
            md="3"
            xl="3"
            sm="1"
          >
            <v-card min-height="400" flat>
              <v-card-title>Servicio</v-card-title>
              <v-card-text>Texto</v-card-text>
              <v-card-actions>
                <v-btn depressed plain>Leer más</v-btn>
              </v-card-actions>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
      </div>
</template>

<style lang="scss" scoped>
.jumbo {
  position: relative;
  &:before,
  &:after {
    content: '';
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
  }
  &:before {
    background-color: #fff;
    background-image: url('~assets/img/pexels-lumn-1028600.jpg');
    background-size: cover;
    z-index: 0;
  }
  &:after {
    background: linear-gradient(transparent, #fff),
      linear-gradient(transparent, #fff), linear-gradient(transparent, #fff),
      rgba(255, 255, 255, 0.6);
    z-index: 0;
  }
}
</style>