<script setup lang="ts">

</script>

<template>
  <section class="multiStepForm__content">
    <div class="multiStepForm__content__header">
      <h2>Personal info</h2>
      <p>Please provide your name, email address and phone number.</p>
    </div>
    <form class="multiStepForm__content__form">
      <div class="multiStepForm__content__form__formGroup">
        <label for="name">Name</label>
        <input id="name" type="text" required placeholder="e.g. Stephen King" />
        <span>Error Msg</span>
      </div>
      <div class="multiStepForm__content__form__formGroup">
        <label for="email">Email Address</label>
        <input id="email" type="email" required placeholder="e.g. stephenking@lorem.com" />
        <span>Error Msg</span>
      </div>
      <div class="multiStepForm__content__form__formGroup">
        <label for="phoneNumber">Phone Number</label>
        <input id="phoneNumber" type="tel" required placeholder="e.g. +1 234 567 890" />
        <span>Error Msg</span>
      </div>
    </form>
    <div class="multiStepForm__content__btnGroup">
      <button class="multiStepForm__content__btnGroup__btn goBackBtn">Go Back</button>
      <button class="multiStepForm__content__btnGroup__btn nextStepBtn">Next Step</button>
    </div>
  </section>
</template>

<style scoped>

</style>