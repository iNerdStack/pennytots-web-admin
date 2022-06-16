<template>
  <v-app light>
    <v-navigation-drawer
      v-model="drawer"
      :mini-variant="miniVariant"
      :clipped="clipped"
      fixed
      app
      color="#1f1e1a"
    >
      <div class="fill-height align-center" style="background-color: #1f1e1a">
        <div class="mt-16 pt-16"></div>
        <v-list
          v-for="item in items"
          :key="item.title"
          class="col-12 ma-0 pa-0"
        >
          <v-list-item
            :to="item.to"
            router
            exact
            class="side_list px-4"
            active-class="side_list"
          >
            <div class="d-flex flex-row py-5">
              <img :src="item.icon" alt="" />
              <span class="ml-2 grey--text">{{ item.title }}</span>
            </div>
          </v-list-item>
        </v-list>
      </div>
    </v-navigation-drawer>
    <v-app-bar :clipped-left="clipped" fixed app color="white" flat>
    </v-app-bar>
    <v-main class="white">
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>

    <v-footer :absolute="!fixed" app>
      <span>&copy; {{ new Date().getFullYear() }} Pennytots.com</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: "DefaultLayout",
  data() {
    return {
      clipped: false,
      drawer: true,
      fixed: false,
      items: [
        {
          icon: "/images/svg/dashboard.svg",
          title: "Dashboard",
          to: "/dashboard",
        },
        {
          icon: "/images/svg/topic.svg",
          title: "Topics",
          to: "/dashboard",
        },
        {
          icon: "/images/svg/comment.svg",
          title: "Chats",
          to: "/dashboard",
        },
        {
          icon: "/images/svg/comment.svg",
          title: "Groups",
          to: "/dashboard",
        },
        {
          icon: "/images/svg/sidebar-user.svg",
          title: "Users",
          to: "/dashboard",
        },
        {
          icon: "/images/svg/sidebar-helpdesk.svg",
          title: "Help Desk",
          to: "/dashboard/helpdesk",
        },
      ],
    };
  },
};
</script>

<style scoped>
.app {
  font-family: "Poppins" !important;
}
body {
  font-family: "Poppins" !important;
}
</style>


<style>
.side_list .v-list-item-group .v-list-item--active {
  background-color: red;
  color: white;
}
</style>