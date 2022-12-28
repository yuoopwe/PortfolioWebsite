<script lang="ts" setup>
import { ref, computed } from 'vue';

const count = ref(1);
const double = computed(() => count.value * 2);
let test: string = 'hello';
test = 1;
</script>

<template>
  <div class="HomePage">
    hello
    <img class="HomePage__laptop" src="/img/laptop.png" />
  </div>
</template>

<style lang="scss" scoped>
.HomePage {
  width: 100%;
  height: 100%;
  background: rgb(39, 41, 50);
  background: linear-gradient(
    90deg,
    rgba(39, 41, 50, 1) 0%,
    rgba(42, 41, 51, 1) 39%,
    rgba(64, 51, 64, 1) 100%
  );

  &__laptop {
    width: 600px;
  }
}
</style>
