<template>
  <v-app>
     <v-main>
         <router-link :to="{ name: 'Home'}"></router-link>
         <router-link :to="{ name: 'About'}"></router-link>
     </v-main>
     <router-view></router-view>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  data: () => ({
    //
  }),
};
</script>
