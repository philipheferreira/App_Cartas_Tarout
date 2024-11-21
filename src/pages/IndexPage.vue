<template>
  <q-page class="flex ">

    <cartas :imagemVersoCarta="img1"></cartas>


  </q-page>
</template>

<script>
import { defineComponent } from 'vue'
import cartas from 'components/Carta.vue'

export default defineComponent({
  name: 'IndexPage',
  components: {
    cartas
  },
  data() {
    return {
      img1: "https://miro.medium.com/v2/resize:fit:720/format:webp/1*Yn5_HWunnZcaPqtrXzc2eQ.jpeg"
    }
  }
})
</script>

<style></style>
