<template>

  <div class="flip-container" @click="isFlipped = !isFlipped">
    <div class="flipper" :class="{ 'flipped': isFlipped }">
      <div class="front">
        <!-- Imagem da frente -->
        <img
          src="https://scontent.fbel7-1.fna.fbcdn.net/v/t39.30808-6/300499300_419109840322194_7374735255376892673_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=cc71e4&_nc_eui2=AeGmSPFXJKbQqtAniqfSPv5yAkfiE9LL6CgCR-IT0svoKEtCNf09bmDYKoOarwVoYrKQvfaoLuV3RX0UzOA5kgOl&_nc_ohc=eOc6LWIoejwQ7kNvgF7SuUV&_nc_zt=23&_nc_ht=scontent.fbel7-1.fna&_nc_gid=AAxpzxjTv8bbWPlszbVUUkm&oh=00_AYC9uvRvEa8eTganjkdRwgjim1xnp0WGddwyTvEO2BjB8Q&oe=67415313"
          alt="Imagem Frente" style="width: 240px; height: 400px" />
      </div>
      <div class="back">
        <!-- Imagem de trás -->
        <img :src="imagemVersoCarta" alt="Imagem Verso" style="width: 240px; height: 400px" />

      </div>
    </div>
  </div>


</template>

<script>
export default {
  name: 'CartasTarot',
  data() {
    return {
      isFlipped: false
    };
  },
  props: {
    imagemVersoCarta: {
      type: String,
      required: true
    },

  }
}
</script>

<style>
.flip-container {
  perspective: 1000px;
  /* Cria um efeito 3D */
  cursor: pointer;
}

.flipper {
  position: relative;
  width: 300px;
  /* Defina a largura desejada */
  height: 200px;
  /* Defina a altura desejada */
  transform-style: preserve-3d;
  transition: transform 0.5s ease-in-out;
}

.flipper.flipped {
  transform: rotateY(180deg);
}

.front,
.back {
  position: absolute;
  width: 100%;
  height: 100%;
  backface-visibility: hidden;
}

.front {
  z-index: 2;
  transform: rotateY(0deg);
}

.back {
  transform: rotateY(180deg);
}
</style>
