<script setup>
import { ClockIcon, ListBulletIcon, ChartBarIcon } from '@heroicons/vue/24/outline'
import NavItem from './NavItem.vue'

const navIteams = {
  timeline: ClockIcon,
  activities: ListBulletIcon,
  progress: ChartBarIcon
}
</script>

<template>
  <nav class="sticky bottom-0 z-10 bg-white text-3xl">
    <ul class="flex items-center justify-around border-t">
     <NavItem v-for="(icon, page) in navIteams" :key="page" >
      <component :is="icon" class="h-6 w-6" /> {{ page }}
    </NavItem>
    </ul>
  </nav>
</template>
