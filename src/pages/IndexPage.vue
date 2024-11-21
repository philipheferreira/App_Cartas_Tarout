<template>
  <q-page class="flex flex-center">

    <cartas></cartas>


  </q-page>
</template>

<script>
import { defineComponent } from 'vue'
import cartas from 'components/Carta.vue'

export default defineComponent({
  name: 'IndexPage',
  data() {
  },
  components: {
    cartas
  }
})
</script>

<style></style>
