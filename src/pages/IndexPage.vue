<template>
  <q-page class="flex flex-center">
    <div class="flip-container" :class="{ 'flipped': isFlipped }" @click="isFlipped = !isFlipped">
      <img alt="Quasar logo" src="~assets/quasar-logo-vertical.svg" style="width: 200px; height: 200px">
    </div>


  </q-page>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'IndexPage',
  data() {
    return {
      isFlipped: false
    };
  }
})
</script>

<style>
.flip-container {
  display: inline-block;
  transition: transform 0.5s ease-in-out;
}

.flipped {
  transform: rotateY(180deg);
}
</style>
