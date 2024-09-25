<script setup lang="ts">

</script>

<template>
  <aside class="multiStepForm__sidebar">

    <div class="multiStepForm__sidebar__element">
      <div class="multiStepForm__sidebar__element__step">
        1
      </div>
      <div class="multiStepForm__sidebar__element__information">
        <p>STEP 1</p>
        <p>YOUR INFO</p>
      </div>
    </div>

    <div class="multiStepForm__sidebar__element">
      <div class="multiStepForm__sidebar__element__step">
        2
      </div>
      <div class="multiStepForm__sidebar__element__information">
        <p>STEP 2</p>
        <p>SELECT PLAN</p>
      </div>
    </div>

    <div class="multiStepForm__sidebar__element">
      <div class="multiStepForm__sidebar__element__step">
        3
      </div>
      <div class="multiStepForm__sidebar__element__information">
        <p>STEP 3</p>
        <p>ADD-ONS</p>
      </div>
    </div>

    <div class="multiStepForm__sidebar__element">
      <div class="multiStepForm__sidebar__element__step">
        4
      </div>
      <div class="multiStepForm__sidebar__element__information">
        <p>STEP 4</p>
        <p>SUMMARY</p>
      </div>
    </div>

  </aside>
</template>

<style scoped>
.multiStepForm__sidebar {
  background-image: url("../assets/images/bg-sidebar-desktop.svg");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: bottom;

  border-radius: 8px;

  display: flex;
  flex-direction: column;
  align-items: baseline;
}

.multiStepForm__sidebar__element {
  display: flex;
  gap: 1rem;
  margin-left: 2rem;
  cursor: pointer;
}

.multiStepForm__sidebar__element:first-of-type {
  margin-top: 2rem;
}

.multiStepForm__sidebar__element__step {
  margin: auto 0;
  width: 30px;
  height: 30px;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
  border: 1px var(--clr-neutral-white) solid;
  color: var(--clr-neutral-white);
}


.multiStepForm__sidebar__element__information p {
  text-transform: uppercase;
}

.multiStepForm__sidebar__element__information p:first-child {
  font-size: 0.75rem;
  letter-spacing: 0.05rem;
}

.multiStepForm__sidebar__element__information p:last-child {
  font-size: 0.9rem;
  color: var(--clr-neutral-white);
  font-weight: 700;
  letter-spacing: 0.15rem;
}

@media screen and (max-width: 768px) {
  .multiStepForm__sidebar {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 15rem;
    border-radius: 0;
    background-image: url("../assets/images/bg-sidebar-mobile.svg");
    background-position: bottom;
    flex-direction: row;
    justify-content: center;
    gap: 1rem;
  }

  .multiStepForm__sidebar__element {
    margin-left: 0;
    margin-top: 3rem;
  }

  .multiStepForm__sidebar__element:first-of-type {
    margin-top: 0;
  }

  .multiStepForm__sidebar__element__information {
    display: none;
  }
}
</style>