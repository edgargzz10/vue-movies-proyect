<template>
  <v-layout class="rounded rounded-md">
    <v-app-bar title="My Movie Ratings"></v-app-bar>

    <v-navigation-drawer>
      <v-list>
        <v-list-item title="Rate movies"></v-list-item>
        <v-list-item title="Add movie"></v-list-item>
        <v-list-item title="Edit movie"></v-list-item>
        <v-list-item title="Delete movie"></v-list-item>

      </v-list>
    </v-navigation-drawer>

    <v-main class="d-flex align-center justify-center" style="min-height: 300px;">
      <router-view></router-view>
    </v-main>
  </v-layout>
</template>

<script setup>
  //
</script>
