<template>
  <main>
    <v-row>
      <v-col cols="12" md="8" class="d-flex flex-column">
        <div class="black">
          <v-tabs class="my-3 black d-flex col-12 ma-0 pa-0 px-4">
            <v-tab class="black"> Topic Updates</v-tab>
            <v-tab class="black white--text"> Reported Topics</v-tab>
            <v-tab class="black white--text"> Removed Topics</v-tab>
          </v-tabs>
        </div>
        <v-row class="mt-5">
          <v-col cols="12" md="6" v-for="i in 6" :key="i">
            <TopicCard />
          </v-col>
        </v-row>
      </v-col>
      <v-col cols="12" md="4" class="d-flex flex-column">
        <div>
          <v-textarea
            label="Type in your tots"
            solo
            color="grey"
            background-color="#F5F5F5"
            flat
          ></v-textarea>
          <hr />
        </div>
        <div class="d-flex flex-column">
          <div
            class="
              col-3
              ma-0
              pa-0
              d-flex
              flex-column
              justify-center
              align-center
              py-3
            "
          >
            <div
              style="border-radius: 10px; width: 30px; height: 30px"
              class="primary d-flex justify-center align-center"
            >
              <v-btn icon color="white"><v-icon> mdi-plus </v-icon> </v-btn>
            </div>

            <span class="grey--text text-12">Attach File</span>
          </div>
          <div class="d-flex flex-column">
            <hr />
            <div class="d-flex align-center mt-2">
              <span class="pr-2 text-12 text-semi-bold"
                >Select relation to this Tot</span
              >
              <v-icon color="red" size="20">mdi-information-outline</v-icon>
            </div>
          </div>
        </div>

        <div class="d-flex mt-3 flex-column">
          <v-row no-gutters>
            <v-col cols="3" class="pa-2">``
              <v-btn outlined block color="black" class="rounded-pill text-none py-6"> ICT</v-btn>
            </v-col>
            <v-col cols="6" class="pa-2">
              <v-btn outlined block color="black" class="rounded-pill text-none py-6"> Agriculture</v-btn>
            </v-col>
              <v-col cols="3" class="pa-2">
              <v-btn outlined block color="black" class="rounded-pill text-none py-6"> Anime</v-btn>
            </v-col>
                <v-col cols="3" class="pa-2">
              <v-btn outlined block color="black" class="rounded-pill text-none py-6">Music</v-btn>
            </v-col>
            <v-col cols="6" class="pa-2">
              <v-btn outlined block color="black" class="rounded-pill text-none py-6"> Banking and Finance</v-btn>
            </v-col>
          </v-row>
          <div class="mt-5">
              <v-btn elevation="0" block color="primary" class="rounded-pill text-none py-6">
                <span class="black--text"> Post</span>
                 </v-btn>
          </div>
        </div>
      </v-col>
    </v-row>
  </main>
</template>

<script>
</script>

<style>
.v-tab {
  text-transform: none !important;
}
hr {
  height: 1px;
  background-color: #ccc;
  border: none;
}
</style>