<template>
  <v-layout class="rounded rounded-md">
    <v-app-bar title="My Movie Ratings"></v-app-bar>

    <v-navigation-drawer>      
      <v-list>
        <v-list-item v-for="(item, index) in items" :key="index" @click="router.push(item.value)" :title="item.title"></v-list-item>
      </v-list>
    </v-navigation-drawer>

    <v-main class="d-flex align-center justify-center" style="min-height: 300px;">
      <router-view></router-view>
    </v-main>
  </v-layout>
</template>

<script setup> 
import router from './router';
  const items = [
    {
      title: 'Rate movies',
      value: '/',
    },
    {
      title: 'Add movie',
      value: '/add',
    }
  ]   
</script>
