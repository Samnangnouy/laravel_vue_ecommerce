<script setup>
import { HomeIcon, UsersIcon, ListBulletIcon, ChartBarIcon } from '@heroicons/vue/24/solid'
</script>

<template>
  <div class="w-[200px] transition-all bg-indigo-700 text-white py-4 px-2">
    <router-link :to="{ name: 'app.dashboard' }"
      class="flex items-center justify-center p-2 rounded transition-colors">
      <img src="../assets/logo.png" alt="Logo" class="w-40 h-40" />
    </router-link>

    <router-link :to="{ name: 'app.dashboard' }"
      class="flex items-center p-2 rounded transition-colors hover:bg-black/30">
      <span class="mr-2 text-gray-300">
        <HomeIcon class="w-5" />
      </span>
      <span class="text-xs">Dashboard</span>
    </router-link>

    <router-link :to="{ name: 'app.products' }" class="flex items-center p-2 rounded transition-colors hover:bg-black/30">
      <span class="mr-2 text-gray-300">
        <ListBulletIcon class="w-5" />
      </span>
      <span class="text-xs">Products</span>
    </router-link>

    <router-link :to="{ name: 'app.dashboard' }"
      class="flex items-center p-2 rounded transition-colors hover:bg-black/30">
      <span class="mr-2 text-gray-300">
        <UsersIcon class="w-5" />
      </span>
      <span class="text-xs">Users</span>
    </router-link>

    <router-link :to="{ name: 'app.dashboard' }"
      class="flex items-center p-2 rounded transition-colors hover:bg-black/30">
      <span class="mr-2 text-gray-300">
        <ChartBarIcon class="w-5" />
      </span>
      <span class="text-xs">Reports</span>
    </router-link>
  </div>
</template>
