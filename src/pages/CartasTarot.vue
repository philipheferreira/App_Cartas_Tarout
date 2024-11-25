<template>
  <div>
    <div class="text-body1 text-center q-ma-md ">Os 22 Arcanos Maiores</div>


    <div class="flex justify-center">
      <div class="q-my-lg q-mx-lg column items-center">
        <img class="imagemCartas" @click="abrirModalOLouco" src="https://www.astrolink.com.br/data/tarot/o-louco.jpg" />
        <Carta_O_Louco ref="OLoucoRef" />
        <div class="text-body2 text-center textoCartas">0 - O Louco</div>
      </div>


      <div class="q-my-lg q-mx-lg column items-center">
        <img class="imagemCartas" @click="abrirModalOMago" src="https://www.astrolink.com.br/data/tarot/o-mago.jpg" />
        <Carta_O_Mago ref="OMagoRef" />
        <div class="text-body2 text-center textoCartas">I - O Mago</div>
      </div>

      <div class="q-my-lg q-mx-lg column items-center">
        <img class="imagemCartas" @click="abrirModalASacerdotisa"
          src="https://www.astrolink.com.br/data/tarot/a-sacerdotisa.jpg" />
        <Carta_A_Sacerdotisa ref="ASacerdotisaRef" />
        <div class="text-body2 text-center textoCartas">II - A Sacerdotisa</div>
      </div>

      <div class="q-my-lg q-mx-lg column items-center">
        <img class="imagemCartas" @click="abrirModalAImperatriz"
          src="https://www.astrolink.com.br/data/tarot/a-imperatriz.jpg" />
        <Carta_A_Imperatriz ref="AImperatrizRef" />
        <div class="text-body2 text-center textoCartas">III - A Imperatriz</div>
      </div>

      <div class="q-my-lg q-mx-lg column items-center">
        <img class="imagemCartas" @click="abrirModalOImperador"
          src="https://www.astrolink.com.br/data/tarot/o-imperador.jpg" />
        <Carta_O_Imperador ref="OImperadorRef" />
        <div class="text-body2 text-center textoCartas">IV - O Imperador</div>
      </div>

      <div class="q-my-lg q-mx-lg column items-center">
        <img class="imagemCartas" @click="abrirModalOPapa" src="https://www.astrolink.com.br/data/tarot/o-papa.jpg" />
        <Carta_O_Papa ref="OPapaRef" />
        <div class="text-body2 text-center textoCartas">V - O Papa</div>
      </div>

      <div class="q-my-lg q-mx-lg column items-center">
        <img class="imagemCartas" src="https://www.astrolink.com.br/data/tarot/os-enamorados.jpg" />
        <div class="text-body2 text-center textoCartas">VI - Os Enamorados</div>
      </div>

      <div class="q-my-lg q-mx-lg column items-center">
        <img class="imagemCartas" src="https://www.astrolink.com.br/data/tarot/o-carro.jpg" />
        <div class="text-body2 text-center textoCartas">VII - O Carro</div>
      </div>

      <div class="q-my-lg q-mx-lg column items-center">
        <img class="imagemCartas" src="https://www.astrolink.com.br/data/tarot/a-forca.jpg" />
        <div class="text-body2 text-center textoCartas">VIII- A forca</div>
      </div>

      <div class="q-my-lg q-mx-lg column items-center">
        <img class="imagemCartas" src="https://www.astrolink.com.br/data/tarot/o-eremita.jpg" />
        <div class="text-body2 text-center textoCartas">IX - O Eremita</div>
      </div>

      <div class="q-my-lg q-mx-lg column items-center">
        <img class="imagemCartas" src="https://www.astrolink.com.br/data/tarot/a-roda-da-fortuna.jpg" />
        <div class="text-body2 text-center textoCartas textoCartas">X - A Roda da Fortuna</div>
      </div>

      <div class="q-my-lg q-mx-lg column items-center">
        <img class="imagemCartas" src="https://www.astrolink.com.br/data/tarot/a-justica.jpg" />
        <div class="text-body2 text-center textoCartas">XI - A Justiça</div>
      </div>

      <div class="q-my-lg q-mx-lg column items-center">
        <img class="imagemCartas" src="https://www.astrolink.com.br/data/tarot/o-enforcado.jpg" />
        <div class="text-body2 text-center textoCartas">XII - O Enforcado</div>
      </div>

      <div class="q-my-lg q-mx-lg column items-center">
        <img class="imagemCartas" src="https://www.astrolink.com.br/data/tarot/a-morte.jpg" />
        <div class="text-body2 text-center textoCartas">XIII - A Morte</div>
      </div>

      <div class="q-my-lg q-mx-lg column items-center">
        <img class="imagemCartas" src="https://www.astrolink.com.br/data/tarot/a-temperanca.jpg" />
        <div class="text-body2 text-center textoCartas">XIV - A Temperança</div>
      </div>

      <div class="q-my-lg q-mx-lg column items-center">
        <img class="imagemCartas" src="https://www.astrolink.com.br/data/tarot/o-diabo.jpg" />
        <div class="text-body2 text-center textoCartas">XV - O Diabo</div>
      </div>

      <div class="q-my-lg q-mx-lg column items-center">
        <img class="imagemCartas" src="https://www.astrolink.com.br/data/tarot/a-torre.jpg" />
        <div class="text-body2 text-center textoCartas">XVI - A Torre</div>
      </div>

      <div class="q-my-lg q-mx-lg column items-center">
        <img class="imagemCartas" src="https://www.astrolink.com.br/data/tarot/a-estrela.jpg" />
        <div class="text-body2 text-center textoCartas">XVII - A Estrela</div>
      </div>

      <div class="q-my-lg q-mx-lg column items-center">
        <img class="imagemCartas" src="https://www.astrolink.com.br/data/tarot/a-lua.jpg" />
        <div class="text-body2 text-center textoCartas">XVIII - A Lua</div>
      </div>

      <div class="q-my-lg q-mx-lg column items-center">
        <img class="imagemCartas" src="https://www.astrolink.com.br/data/tarot/o-sol.jpg" />
        <div class="text-body2 text-center textoCartas">XIX - O Sol</div>
      </div>

      <div class="q-my-lg q-mx-lg column items-center">
        <img class="imagemCartas" src="https://www.astrolink.com.br/data/tarot/o-julgamento.jpg" />
        <div class="text-body2 text-center textoCartas">XX - O Julgamento</div>
      </div>

      <div class="q-my-lg q-mx-lg column items-center">
        <img class="imagemCartas" src="https://www.astrolink.com.br/data/tarot/o-mundo.jpg" />
        <div class="text-body2 textoCartas">XXI - O Mundo</div>
      </div>

    </div>

  </div>
</template>

<script>
import Carta_O_Louco from '../modal/infoCartas/1_OLouco.vue'
import Carta_O_Mago from '../modal/infoCartas/2_OMago.vue'
import Carta_A_Sacerdotisa from '../modal/infoCartas/3_ASacerdotisa.vue'
import Carta_A_Imperatriz from '../modal/infoCartas/4_AImperatriz.vue'
import Carta_O_Imperador from '../modal/infoCartas/5_OImperador.vue'
import Carta_O_Papa from '../modal/infoCartas/6_OPapa.vue'
import Carta_Os_Enamorados from '../modal/infoCartas/7_OsEnamorados.vue'
import Carta_O_Carro from '../modal/infoCartas/8_OCarro.vue'
import Carta_A_Forca from '../modal/infoCartas/9_AForca.vue'
import Carta_O_Eremita from '../modal/infoCartas/10_OEremita.vue'

export default {
  name: 'CartasTarot',
  components: {
    Carta_O_Louco,
    Carta_O_Mago,
    Carta_A_Sacerdotisa,
    Carta_A_Imperatriz,
    Carta_O_Imperador,
    Carta_O_Papa,
    Carta_Os_Enamorados,
    Carta_O_Carro,
    Carta_A_Forca,
    Carta_O_Eremita
  },
  methods: {
    abrirModalOLouco() {
      this.$refs.OLoucoRef.openDialog(); // Chama o método do componente filho
    },
    abrirModalOMago() {
      this.$refs.OMagoRef.openDialog(); // Chama o método do componente filho
    },
    abrirModalASacerdotisa() {
      this.$refs.ASacerdotisaRef.openDialog(); // chama o método do componente filho
    },
    abrirModalAImperatriz() {
      this.$refs.AImperatrizRef.openDialog(); // chama o método do componente filho
    },
    abrirModalOImperador() {
      this.$refs.OImperadorRef.openDialog(); // chama o método do componente filho
    },
    abrirModalOPapa() {
      this.$refs.OPapaRef.openDialog(); // chama o método do componente filho
    },
    abrirModalOsEnamorados() {
      this.$refs.OsEnamoradosRef.openDialog(); // chama o método do componente filho
    },
    abrirModalOCarro() {
      this.$refs.OCarroRef.openDialog(); // chama o método do componente filho
    },
    abrirModalAForca() {
      this.$refs.AForcaRef.openDialog(); // chama o método do componente filho
    },
    abrirModalOEremita() {
      this.$refs.OEremitaRef.openDialog(); // chama o método do componente filho
    }

  }
}
</script>

<style>
.imagemCartas {
  max-height: 80%;
  max-width: 70%;
  min-height: 160px;
  min-width: 100px;
}

.imagemCartas:hover {
  cursor: pointer;
}

.textoCartas {
  max-width: 100px;
}
</style>
