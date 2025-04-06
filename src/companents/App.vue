<template>
  <div>
    <Header :searchQuery="searchQuery" @update:searchQuery="searchQuery = $event" />
    <router-view :searchQuery="searchQuery" />
  </div>
</template>

<script setup>
import { ref } from 'vue'
import Header from '@/companents/header.vue'

const searchQuery = ref('')
</script>
