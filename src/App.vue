<template>
  <v-layout class="rounded rounded-md">
    <v-app-bar title="My Movie Ratings"></v-app-bar>

    <v-navigation-drawer>      
      <v-list :items="items"></v-list>
    </v-navigation-drawer>

    <v-main class="d-flex align-center justify-center" style="min-height: 300px;">
      <router-view></router-view>
    </v-main>
  </v-layout>
</template>

<script setup> 
  const items = [
    {
      title: 'Rate movies',
      value: 1,
    },
    {
      title: 'Add movie',
      value: 2,
    }
  ]   
</script>
