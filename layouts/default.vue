<template>
  <v-app id="inspire">
    <v-app-bar 
      color="transparent"
      fixed
    >
      <img src="../photos/logo_pets.png" alt="" height="95%" class="ma-2" style="margin:100px">

      <v-btn
        text
      >
        About
      </v-btn>
      <v-btn
        text
      >
        New Flim
      </v-btn>
      <v-btn
        text
      >
        Infor
      </v-btn>
      <v-spacer></v-spacer>
      <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>
      <v-btn icon>
        <v-icon>mdi-account</v-icon>
      </v-btn>
      <v-menu
        left
        bottom
      >
        <template v-slot:activator="{ on, attrs }">
          <v-btn
            icon
            v-bind="attrs"
            v-on="on"
          >
            <v-icon>mdi-dots-vertical</v-icon>
          </v-btn>
        </template>

        <v-list class="mt-6">
          <v-list-item
            v-for="n in 5"
            :key="n"
            @click="() => {}"
          >
            <v-list-item-title>Option {{ n }}</v-list-item-title>
          </v-list-item>
        </v-list>
      </v-menu>
    </v-app-bar>

    <v-navigation-drawer
      v-model="drawer"
      fixed
      temporary
    >
      <!--  -->
    </v-navigation-drawer>

    <Nuxt />

    <v-footer
      padless
      width="100vw"
    >
      <v-card
        flat
        tile
        class=" white--text text-center"
        width="100vw"
        align="center"
        justify="center"
      >
      <v-row align="center" justify="center" width="auto" d-block>

        <img src="../photos/Logo pets.png" alt="" height="80px" class="ma-5">
        <div  style="width: 40vw; margin: 16px">
          
        <v-card-text class="white--text pt-0 mt-3" >
           Phasellus feugiat arcu sapien, et iaculis ipsum elementum sit amet. Mauris cursus commodo interdum. Praesent ut risus eget metus luctus accumsan id ultrices nunc. Sed at orci sed massa consectetur dignissim a sit amet dui. Duis commodo vitae velit et faucibus. Morbi vehicula lacinia malesuada. Nulla placerat augue vel ipsum ultrices, cursus iaculis dui sollicitudin. Vestibulum eu ipsum vel diam elementum tempor vel ut orci. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.
        </v-card-text>
        </div>
      </v-row>

        <v-divider></v-divider>

        <v-card-text class="white--text">
          {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
        </v-card-text>
      </v-card>
    </v-footer>
  </v-app>
</template>

<script>
  export default {
    data: () => ({ 
      drawer: null,
      icons: [
      'mdi-facebook',
      'mdi-twitter',
      'mdi-linkedin',
      'mdi-instagram',
      ],
      }),
  }
</script>

<style>

</style>
