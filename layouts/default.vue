<template>
  <v-app id="inspire">
    <v-app-bar 
      color="transparent"
      fixed
    >
      <img src="../photos/anthonymovie.png" alt="" height="80%" class="ma-2">

      <v-btn
        text
        :key="1"
      >
        About
      </v-btn>
      <v-btn
        text
        :key="1"
      >
        New Flim
      </v-btn>
      <v-btn
        text
        :key="1"
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

    <v-main class="grey lighten-2">
      <v-carousel hide-delimiters height="100vh">
        <v-carousel-item
          v-for="(item,i) in items"
          :key="i"
          :src="item.src"
        ></v-carousel-item>
      </v-carousel>
      <v-container >
        <v-row color="grey darken-3">
          <template >
            <v-col
              class="mt-2"
              cols="12"
            >
              <strong>Category 2</strong>
            </v-col>

            <v-col
              v-for="j in 6"
              :key="j"
              cols="6"
              md="2"
            >
              <v-sheet height="150" align="center" justify="center" class="fill-height"> hello</v-sheet>
            </v-col>
          </template>
        </v-row>
      </v-container>
      <v-card color="blue-grey" height="100vh" >
        <v-card-text>
          hellowrd
        </v-card-text>
        
      </v-card>
      <v-container >
        <v-row color="grey darken-3">
          <template >
            <v-col
              class="mt-2"
              cols="12"
            >
              <strong>Category 2</strong>
            </v-col>

            <v-col
              v-for="j in 6"
              :key="j"
              cols="6"
              md="2"
            >
              <v-sheet height="150" align="center" justify="center" class="fill-height"> hello</v-sheet>
            </v-col>
          </template>
        </v-row>
      </v-container>
      <v-card  >
        <v-card-text>
          hellowrd
        </v-card-text>
        
      </v-card>
      <v-container >
        <v-row color="grey darken-3">
          <template >
            <v-col
              class="mt-2"
              cols="12"
            >
              <strong>Category 2</strong>
            </v-col>

            <v-col
              v-for="j in 6"
              :key="j"
              cols="6"
              md="2"
            >
              <v-sheet height="150" align="center" justify="center" class="fill-height"> hello</v-sheet>
            </v-col>
          </template>
        </v-row>
      </v-container>
    </v-main>
    
    <v-main>

    </v-main>
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

        <img src="../photos/anthonymovie.png" alt="" height="80px" class="ma-2">
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
      items: [
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg',
          },
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/sky.jpg',
          },
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/bird.jpg',
          },
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/planet.jpg',
          },
        ],
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
