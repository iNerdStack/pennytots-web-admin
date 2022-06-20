<template>
  <div>
    <v-row>
      <v-col cols="12" md="4" class="px-3">
        <div class="d-flex flex-column">
          <div class="d-flex justify-center">
            <div
              class="pa-4 d-flex flex-row col-md-12"
              style="border-radius: 20px; background-color: #2e2e2e"
            >
              <div>
                <img
                  src="/images/svg/comment.svg"
                  width="20px"
                  alt=""
                  class="mr-2"
                  style="padding-top: 2px"
                />
              </div>

              <div>
                <span class="font-weight-bold text-14 white--text">Chats</span>
              </div>
            </div>
          </div>
          <v-tabs class="mt-5">
            <v-tab>Reported Chats</v-tab>
            <v-tab>My Chats</v-tab>
          </v-tabs>

          <v-row class="mt-2" no-gutters>
            <v-col
              cols="12"
              v-for="(item, index) in 10"
              :key="index"
              class="mb-1"
            >
              <div>
                <div>
                  <div height="100%" class="pa-1 d-flex flex-row">
                    <div class="d-flex flex-row">
                      <div>
                        <img src="/images/profile-2.jpg" alt="" />
                      </div>
                    </div>

                    <div class="d-flex flex-column ml-3">
                      <span class="text-semi-bold">Jerome Bell</span>
                      <p class="text-13">
                        Dave I need help with a nature assignment..
                      </p>
                    </div>
                  </div>
                </div>
              </div>
            </v-col>
          </v-row>
        </div>
      </v-col>
      <v-col cols="12" md="8" class="d-flex align-center justify-center">
        <div class="d-flex align-center justify-center flex-column">
          <img src="/images/svg/chats-bg.svg" alt="" />
          <div class="d-flex flex-column text-center">
            <span class="my-2 text-20">Send, recieve & manage groups </span>
            <div class="text-center d-flex align-center justify-center">
              <div class="col-12 col-md-8 ma-0 pa-0">
                <span class="text-12"
                  >Tristique posuere ut pellentesque duis aliquet nam. Iaculis
                  nec non adipiscing enim, euismod pellentesque nunc. Blandit
                  diam rhoncus, eget consequat, aliquam tortor senectus morbi.
                  Id facilisi vel pretium</span
                >
              </div>
            </div>
          </div>
        </div>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {};
</script>

<style>
</style>