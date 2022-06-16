<template>
  <main>
    <v-row>
      <v-col cols="8" class="d-flex flex-column px-4">
        <div class="d-flex flex-row">
          <v-card
            height="170px"
            width="270px"
            v-for="(item, index) in stats"
            :key="index"
            class="d-flex justify-center align-center mx-2"
            elevation="1"
          >
            <div class="d-flex flex-row">
              <div class="d-flex justify-center align-center">
                <div
                  class="d-flex pa-4"
                  :style="`border-radius: 30px; background-color: ${item.color}`"
                >
                  <img src="/images/svg/stats-icon.svg" alt="" />
                </div>
              </div>

              <div class="d-flex flex-column pl-3">
                <span class="text-16 text-semi-bold">{{ item.title }}</span>
                <span class="text-30">{{ item.count }}</span>
              </div>
            </div>
          </v-card>
        </div>

        <v-row>
          <v-col cols="12" md="6">
            <div>
              <div class="mt-16 d-flex flex-column ml-3">
                <span>Help Desk messages</span>
                <div
                  style="height: 360px; background-color: #f3f4f7"
                  class="mt-3 d-flex flex-column"
                >
                  <img
                    src="/images/svg/chart.svg"
                    alt=""
                    width="250px"
                    class="pa-4"
                  />
                  <div class="d-flex flex-row mt-3 px-5">
                    <div class="d-flex flex-column">
                      <div class="d-flex flex-row align-center mr-16">
                        <div
                          style="
                            background-color: #006b7a;
                            border-radius: 10px;
                            padding: 10px;
                          "
                        ></div>
                        <span
                          class="text-14 ml-1 text-10"
                          style="margin-top: 3px; color: #696969"
                        >
                          Read</span
                        >
                      </div>
                      <span
                        class="text-30 text-semi-bold"
                        style="color: #696969"
                        >3,000</span
                      >
                    </div>
                    <div class="d-flex flex-column">
                      <div class="d-flex flex-row align-center">
                        <div
                          style="border-radius: 10px; padding: 10px"
                          class="highlight"
                        ></div>
                        <span
                          class="text-14 ml-1 text-10"
                          style="margin-top: 3px; color: #696969"
                        >
                          Unread</span
                        >
                      </div>

                      <span
                        class="text-30 text-semi-bold"
                        style="color: #696969"
                        >1,000</span
                      >
                    </div>
                  </div>
                </div>
              </div>

              <div class="d-flex flex-column mt-7 ml-3">
                <span
                  >Unread help desk messages
                  <span class="primary--text">(5) </span></span
                >

                <v-row class="mt-1" no-gutters>
                  <v-col
                    cols="12"
                    v-for="(item, index) in 3"
                    :key="index"
                    class="mb-2"
                  >
                    <div style="background-color: #f3f4f7">
                      <div height="100%" class="pa-3 d-flex flex-row">
                        <div class="d-flex flex-row">
                          <div>
                            <img src="/images/profile-2.jpg" alt="" />
                          </div>
                        </div>

                        <div class="d-flex flex-column ml-3">
                          <span class="text-semi-bold">Kathryn Murphy</span>
                          <p class="text-13">
                            Do you know that peakcock besides being the national
                            bird of India, peacocks have been part of Greek
                            mythology.
                          </p>
                        </div>
                      </div>
                    </div>
                  </v-col>
                </v-row>
              </div>
            </div>
          </v-col>

          <!-- Activities -->
          <v-col cols="12" md="6">
            <div>
              <div class="mt-16 d-flex flex-column ml-3">
                <span>Activities</span>
                <v-row class="mt-4">
                  <v-col
                    cols="12"
                    class="d-flex flex-row align-center pa-3"
                    v-for="(item, index) in 10"
                    :key="index"
                  >
                    <div>
                      <img src="/images/profile-2.jpg" alt="" />
                    </div>

                    <span class="text-12 ml-2 mb-1"
                      >David Adegoke sends New help desk message</span
                    >
                  </v-col>
                </v-row>
              </div>
            </div>
          </v-col>
        </v-row>
      </v-col>
      <v-col cols="4" class="px-3">
        <div class="d-flex flex-column">
          <div class="d-flex justify-center">
            <div
              class="pa-4 d-flex flex-row col-md-11"
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
              v-for="(item, index) in 5"
              :key="index"
              class="mb-2"
            >
              <div class="chat-card">
                <div>
                  <div height="100%" class="pa-3 d-flex flex-row">
                    <div class="d-flex flex-row">
                      <div>
                        <img src="/images/profile-2.jpg" alt="" />
                      </div>
                    </div>

                    <div class="d-flex flex-column ml-3">
                      <span class="text-semi-bold">Jerome Bell</span>
                      <p class="text-13">
                        Devil is harrassing me in an un explanable way
                      </p>
                      <div
                        class="highlight d-flex flex-column pa-2"
                        style="border-radius: 4px"
                      >
                        <span class="text-semi-bold text-10 white--text">
                          Guy Hawkins >> Leslie Alexander</span
                        >
                        <div class="d-flex flex-row align-center">
                          <span class="text-10 primary--text">
                            View conversation</span
                          >
                          <v-icon color="primary">mdi-arrow-right</v-icon>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </v-col>
          </v-row>
        </div>
      </v-col>
    </v-row>
  </main>
</template>

<script>
export default {
  data: () => ({
    stats: [
      {
        id: 1,
        color: "#3EC37F",
        title: "Total Users",
        count: "3.1k",
      },
      {
        id: 2,
        color: "#F6BC65",
        title: "Total Users",
        count: "3.1k",
      },
      {
        id: 3,
        color: "#5BA2F6",
        title: "Total Topics",
        count: "3.1k",
      },
    ],
  }),
};
</script>

<style>
.v-tab {
  text-transform: none !important;
}
.chat-card {
  border-left: 5px solid #f19c4a;
  background-color: #fef0e3;
}
</style>