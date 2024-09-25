<script setup lang="ts">

import Sidebar from "@/components/Sidebar.vue";
import Step1 from "@/components/Step1.vue";
import Step2 from "@/components/Step2.vue";
</script>




<template>
  <div class="center-container">
    <main class="multiStepForm">
      <h1 class="sr-only">Multi Step Form</h1>
      <Sidebar />
<!--      <Step1 />-->
      <Step2 />
    </main>
  </div>
</template>



<style scoped>

</style>