<template>
  <v-system-bar window>
    <v-menu offset-y transition="slide-y-transition">
      <v-btn flat small right slot="activator">
        <v-icon>headset</v-icon> Acerca de
      </v-btn>
      <v-list>
        <v-list-tile @click="dialog = true">
          <v-list-tile-title>Pozole Verde</v-list-tile-title>
        </v-list-tile>
        <v-dialog v-model="dialog" max-width="300">
          <v-card>
            <v-card-title><h2>Equipo Pozole Verde</h2></v-card-title>
            <v-card-text>Musica por www.bensound.com</v-card-text>
            <v-card-actions>
              <v-spacer></v-spacer>
              <v-btn flat @click="dialog = false">OK</v-btn>
            </v-card-actions>
          </v-card>
        </v-dialog>
      </v-list>
    </v-menu>
    <v-spacer></v-spacer>
    POZOLE VERDE
    <v-spacer></v-spacer>
    <v-icon>remove</v-icon>
    <v-icon>check_box_outline_blank</v-icon>
    <v-icon>close</v-icon>
  </v-system-bar>
</template>

<script>
  export default {
    data () {
      return {
        dialog: false
      }
    },
  }
</script>
