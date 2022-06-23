<template>
  <main>
    <v-row>
      <v-col cols="12" md="6" class="fill-height">
        <div class="d-flex justify-center align-center" style="height: 98vh">
          <div class="flex-column d-flex col-12 col-md-7">
            <div class="d-flex justify-center">
              <img src="/images/svg/logo.svg" alt="" />
            </div>

            <div class="mt-4">
              <span class="text-15 text-semi-bold">Email Address</span>
              <v-text-field
                placeholder="example@gmail.com"
                solo
                color="grey"
                background-color="#F5F5F5"
                flat
                class="mt-1"
              ></v-text-field>
            </div>
            <div class="mt-2">
              <span class="text-15 text-semi-bold">Password</span>
              <v-text-field
                solo
                color="grey"
                background-color="#F5F5F5"
                flat
                :append-icon="showPassword ? 'mdi-eye' : 'mdi-eye-off'"
                class="mt-1 input-group--focused"
                :type="showPassword ? 'text' : 'password'"
                name="input-10-2"
                label="Not visible"
                hint="At least 8 characters"
                @click:append="showPassword = !showPassword"
              ></v-text-field>
            </div>
            <div class="mt-3">
              <v-btn
                elevation="0"
                block
                color="accent"
                class="rounded-pill text-none py-6"
              >
                <span class="primary--text"> Post</span>
              </v-btn>
            </div>
          </div>
        </div>
      </v-col>
      <v-col cols="12" md="6">
        <div class="d-flex fill-height justify-center align-center pa-6">
          <div class="d-flex justify-end">
            <img src="/images/svg/side-login.svg" width="75%" alt="" />
          </div>
        </div>
      </v-col>
    </v-row>
  </main>
</template>

<script>
export default {
  layout: "empty",
  data: () => ({
    showPassword: false,
  }),
};
</script>

<style>
</style>