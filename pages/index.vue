<template>
    <v-main class="black" >
      
      <v-card 
      style="height:100vh; width: 100vw; overflow:hidden; position: relative"  
      class="d-flex flex-column justify-end"
      >
        <v-img 
        src="https://cdn.mos.cms.futurecdn.net/VQxFwgrZNNFJwo7pCtMesD.jpg" 
        width="100vw"
        height="100%"
        style="position:absolute"
        alt=""
        >
        </v-img>
        <v-card 
        style="position:relative;" 
        class="text-capitalize ma-10 white--text font-weight-black d-flex flex-column justify-end" 
        align-self="end" 
        color="transparent"
        flat
        >
          <v-col>
          <div class="text-h4 font-weight-black">

          War for the Planet of the Apes
          </div>
          <div style="width:50%">
            Deep in the Muir woods, soldiers stalk through accompanied by a band deserter Apes, each identified with Donkey inscribed on their backs and slogans such as Monkey Killer on their helmets.  They also have AΩ branded on their foreheads to identify them as part of the alpha-omega devision.
          </div>
          <v-btn
            color="error"
          >
            Get Infor
          </v-btn>
          </v-col>
        </v-card>
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
</template>

<script>
export default {
  computed:{
    header() {
      return this.$store.state.post.basic
    }
  },
}
</script>
