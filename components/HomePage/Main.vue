<script lang="ts" setup>
import { ref, computed } from 'vue';

const count = ref(1);
const double = computed(() => count.value * 2);
</script>

<template>
  <div class="HomePage">
    <HomePageSideNav />
    <div class="HomePage__content">
      <HomePageButtonNav />
      <img
        class="HomePage__laptopImage"
        alt="image of laptop"
        src="/img/laptop.png"
      />
    </div>
  </div>
</template>

<style lang="scss" scoped>
.HomePage {
  display: flex;
  width: 100%;
  height: 100%;
  background: rgb(39, 41, 50);
  background: linear-gradient(
    90deg,
    rgba(39, 41, 50, 1) 0%,
    rgba(42, 41, 51, 1) 39%,
    rgba(64, 51, 64, 1) 100%
  );

  &__content {
    width: 100%;
  }

  &__laptopImage {
    position: relative;
    width: 600px;
    height: 380px;
    z-index: 0;
  }
}
</style>
