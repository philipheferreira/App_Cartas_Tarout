<template>
  <q-page class="flex justify-center q-mt-lg">

    <cartas :imagemVersoCarta="img1"></cartas>
    <cartas :imagemVersoCarta="img2"></cartas>
    <cartas :imagemVersoCarta="img3"></cartas>
    <cartas :imagemVersoCarta="img4"></cartas>
    <cartas :imagemVersoCarta="img5"></cartas>
    <cartas :imagemVersoCarta="img6"></cartas>
    <cartas :imagemVersoCarta="img7"></cartas>
    <cartas :imagemVersoCarta="img8"></cartas>
    <cartas :imagemVersoCarta="img9"></cartas>
    <cartas :imagemVersoCarta="img10"></cartas>
    <cartas :imagemVersoCarta="img11"></cartas>
    <cartas :imagemVersoCarta="img12"></cartas>
    <cartas :imagemVersoCarta="img13"></cartas>
    <cartas :imagemVersoCarta="img14"></cartas>
    <cartas :imagemVersoCarta="img15"></cartas>
    <cartas :imagemVersoCarta="img16"></cartas>
    <cartas :imagemVersoCarta="img17"></cartas>
    <cartas :imagemVersoCarta="img18"></cartas>
    <cartas :imagemVersoCarta="img19"></cartas>
    <cartas :imagemVersoCarta="img20"></cartas>
    <cartas :imagemVersoCarta="img21"></cartas>
    <cartas :imagemVersoCarta="img22"></cartas>

  </q-page>
</template>

<script>
import { defineComponent } from 'vue'
import cartas from 'components/Carta.vue'

export default defineComponent({
  name: 'JogoTarot',
  components: {
    cartas
  },
  data() {
    return {
      img1: "https://www.astrolink.com.br/data/tarot/o-louco.jpg",
      img2: "https://www.astrolink.com.br/data/tarot/o-mago.jpg",
      img3: "https://www.astrolink.com.br/data/tarot/a-sacerdotisa.jpg",
      img4: "https://www.astrolink.com.br/data/tarot/a-imperatriz.jpg",
      img5: "https://www.astrolink.com.br/data/tarot/o-imperador.jpg",
      img6: "https://www.astrolink.com.br/data/tarot/o-papa.jpg",
      img7: "https://www.astrolink.com.br/data/tarot/os-enamorados.jpg",
      img8: "https://www.astrolink.com.br/data/tarot/o-carro.jpg",
      img9: "https://www.astrolink.com.br/data/tarot/a-forca.jpg",
      img10: "https://www.astrolink.com.br/data/tarot/o-eremita.jpg",
      img11: "https://www.astrolink.com.br/data/tarot/a-roda-da-fortuna.jpg",
      img12: "https://www.astrolink.com.br/data/tarot/a-justica.jpg",
      img13: "https://www.astrolink.com.br/data/tarot/o-enforcado.jpg",
      img14: "https://www.astrolink.com.br/data/tarot/a-morte.jpg",
      img15: "https://www.astrolink.com.br/data/tarot/a-temperanca.jpg",
      img16: "https://www.astrolink.com.br/data/tarot/o-diabo.jpg",
      img17: "https://www.astrolink.com.br/data/tarot/a-torre.jpg",
      img18: "https://www.astrolink.com.br/data/tarot/a-estrela.jpg",
      img19: "https://www.astrolink.com.br/data/tarot/a-lua.jpg",
      img20: "https://www.astrolink.com.br/data/tarot/o-sol.jpg",
      img21: "https://www.astrolink.com.br/data/tarot/o-julgamento.jpg",
      img22: "https://www.astrolink.com.br/data/tarot/o-mundo.jpg"

    }
  }
})
</script>

<style></style>
