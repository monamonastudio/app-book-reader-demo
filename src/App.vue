<script setup lang="ts">
import AppNavBar from "@/components/App/AppNavBar.vue";
import AppContent from "./components/App/AppContent.vue";
import AppBottomTabs from "@/components/App/AppBottomTabs.vue";
</script>

<template>
  <div class="border w-fit">
    <div class="max-w-[400px] top-0 h-screen relative">
      <AppNavBar />
      <AppContent>
        <RouterView />
      </AppContent>
      <AppBottomTabs />
    </div>
  </div>
</template>