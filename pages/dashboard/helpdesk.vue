<template>
  <main>
    <div class="mx-5">
      <div class="custom-header pa-5 d-flex flex-row">
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
          <span class="font-weight-bold text-14 white--text">Help Desk</span>
        </div>
      </div>

      <div
        class="d-flex flex-row mt-6 mx-2 col-12 col-md-4 justify-space-between"
      >
        <div class="d-flex flex-row">
          <img src="/images/svg/back-icon.svg" width="18" alt="" />
          <span class="highlight--text text-14 text-semi-bold ml-3"
            >Go back</span
          >
        </div>
        <div class="d-flex flex-row">
          <img src="/images/svg/unarchived.svg" width="18" alt="" />
          <span class="highlight--text text-14 text-semi-bold ml-3"
            >Unarchived</span
          >
        </div>
        <div class="d-flex flex-row">
          <img src="/images/svg/read.svg" width="18" alt="" />
          <span class="highlight--text text-14 text-semi-bold ml-3"
            >Mark Read</span
          >
        </div>
      </div>

      <hr />

      <v-row>
        <v-col cols="4"> </v-col>
        <v-col cols="7">
          <v-card color="white" height="100%" class="pa-5 d-flex flex-row">
            <div class="d-flex flex-row">
              <div>
                <img src="/images/profile.jpg" alt="" />
              </div>
            </div>

            <div class="d-flex flex-column ml-3">
              <span class="text-semi-bold">Jacob Jones</span>
              <p class="text-14">
                Arcu sed massa arcu, placerat. Sit tellus lectus arcu pretium
                erat nulla mattis ultrices donec. Nullam sem diam varius nunc.
                Sed nunc morbi in facilisi. Habitasse arcu euismod faucibus
                lectus arcu. Massa nunc, eget nec vulputate tellus euismod ut.
                Consectetur lacus at auctor ultricies odio sem eu, et leo.
                Mauris, risus arcu nam diam mi a arcu egestas. Quis ac gravida
                nec ultricies nunc, duis vitae eget enim. Odio eget volutpat
                urna, quam commodo elementum tempus enim faucibus. Turpis id
                blandit vitae risus. Mollis feugiat semper pellentesque rhoncus
                quis molestie facilisis sed morbi. Mollis nunc morbi cras
                dignissim massa. At facilisis faucibus amet, amet. Elit sodales
                interdum sit ullamcorper interdum. Id auctor ut sodales dictumst
                sociis euismod ac. Massa dictum iaculis id convallis odio
                turpis. Proin lacus augue tincidunt nam arcu eros sed. Arcu
                volutpat elit eget consectetur quam nunc interdum at. Turpis
                cras integer posuere sit habitant ultrices viverra viverra
                lacus.
              </p>
            </div>
          </v-card>
        </v-col>
        <v-col cols="1"> </v-col>
      </v-row>
    </div>
  </main>
</template>

<script>
export default {};
</script>

<style>
.custom-header {
  border-top-left-radius: 16px;
  border-bottom-left-radius: 16px;
  background-color: #2e2e2e;
}
</style>