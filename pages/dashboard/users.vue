<template>
  <main>
    <div class="mx-5 d-flex flex-column">
      <div class="custom-header pa-5 d-flex flex-row">
        <div>
          <img
            src="/images/svg/users.svg"
            width="20px"
            alt=""
            class="mr-2"
            style="padding-top: 2px"
          />
        </div>

        <div>
          <span class="font-weight-bold text-14 white--text">Users</span>
        </div>
      </div>

      <div class="mt-8" id="content-list">
        <table width="100%">
          <thead class="pa-5" style="background-color: #f7f8fa">
            <th width="30%" class="py-2 pl-2">
              <div class="d-flex">
                <span class="text-regular"> Name</span>
              </div>
            </th>
            <th width="10%">
              <div class="d-flex"><span class="text-regular"> Role</span></div>
            </th>
            <th width="20">
              <div class="d-flex">
                <span class="text-regular"> Last Active</span>
              </div>
            </th>
            <th width="40"></th>
          </thead>
          <tr v-for="(item, index) in users" :key="index" class="py-2">
            <td class="py-3">
                <div class="d-flex flex-row">
  <div>
    <img src="/images/profile.png" width="20px" alt="">
  </div>
  <div class="d-flex flex-column pl-3">
   <span class="text-12 text-semi-bold"> {{ item.name }}</span>
    <span class="text-12"> {{ item.email }}</span>
  </div>
                </div>
           
            </td>
            <td class="text-12">{{ item.role }}</td>
            <td>
              <span class="text-12"> {{ item.lastActive }} </span>
            </td>
            <td>
              <div class="d-flex flex-row justify-center">
                <div class="d-flex flex-row align-center">
                  <div
                    style="height: 10px; width: 10px; border-radius: 10px"
                    :class="`${item.status == 'Active' ? 'green' : 'red'} mr-2`"
                  ></div>
                  <span class="text-12">{{item.status}}</span>
                </div>

                <div class="d-flex flex-row align-center pl-5">
                  <v-icon size="20">mdi-eye</v-icon>
                  <span class="text-12 ml-2">View</span>
                </div>

                <div class="d-flex flex-row align-center pl-5">
                  <v-icon size="20">mdi-clipboard-text</v-icon>
                  <span class="text-12 ml-2">Activities</span>
                </div>

                <div class="d-flex flex-row align-center pl-5">
                  <v-icon size="20">mdi-table-edit</v-icon>
                  <span class="text-12 ml-2">Edit</span>
                </div>
              </div>
            </td>
          </tr>
        </table>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  data: () => ({
    users: [
      {
        id: 1,
        name: "John Doe",
        email: "joe@gmail.com",
        role: "Admin",
            lastActive: "2 days ago",
        status: "Active"
        },
        {
        id: 2,
        name: "Ojo Mehn",
        email: "kemper@gmail.com",
        role: "Manager",
        lastActive: "8 days ago",
         status: "Disabled"
          },
             {
        id: 3,
        name: "Wonder Woman",
        email: "wWoman@gmail.com",
        role: "User",
        lastActive: "8 days ago",
         status: "Disabled"
          },
             {
        id: 2,
        name: "Ojo Mehn",
        email: "kemper@gmail.com",
        role: "Manager",
        lastActive: "4 days ago",
         status: "Active"
          },
             {
        id: 2,
        name: "Ojo Mehn",
        email: "kemper@gmail.com",
        role: "Manager",
        lastActive: "8 days ago",
         status: "Disabled"
          },
             {
        id: 2,
        name: "Ojo Mehn",
        email: "kemper@gmail.com",
        role: "Manager",
        lastActive: "8 days ago",
         status: "Disabled"
          },
             {
        id: 2,
        name: "Ojo Mehn",
        email: "kemper@gmail.com",
        role: "Manager",
        lastActive: "8 days ago",
         status: "Disabled"
        },
      
    ],
  }),
};
</script>

<style>
.custom-header {
  border-top-left-radius: 16px;
  border-bottom-left-radius: 16px;
  background-color: #2e2e2e;
}

#content-list table {
  width: 100%;
}

#content-list td,
th {
  border: 1px solid #f2f2f2;
  text-align: left;
  padding: 8px;
}

#content-list tr:nth-child(2n + 1) {
  background-color: #f2f2f2;
}

#content-list tr {
  padding: 8px;
}
</style>