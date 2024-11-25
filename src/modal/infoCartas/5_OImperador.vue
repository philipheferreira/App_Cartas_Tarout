<template>

  <q-dialog v-model="isOpen" transition-show="rotate" transition-hide="rotate">
    <q-card style="max-width: 70%;">
      <q-card-section>
        <div class="text-h6">IV - O Imperador</div>
      </q-card-section>

      <q-card-section>
        Informações sobre a carta O Imperador
      </q-card-section>

      <q-separator />

      <q-card-section style="max-height: 50vh" class="scroll">
        <p v-for="n in 15" :key="n">Lorem ipsum dolor sit amet consectetur adipisicing elit. Rerum repellendus sit
          voluptate voluptas eveniet porro. Rerum blanditiis perferendis totam, ea at omnis vel numquam exercitationem
          aut, natus minima, porro labore.</p>
      </q-card-section>

      <q-separator />

      <q-card-actions align="right">
        <q-btn flat label="Fechar" color="accent" @click="closeDialog" />
      </q-card-actions>
    </q-card>
  </q-dialog>

</template>

<script>
export default {


  data() {
    return {
      isOpen: false // Estado de abertura do diálogo
    };
  },
  methods: {
    openDialog() {
      this.isOpen = true; // Abre o diálogo
    },
    closeDialog() {
      this.isOpen = false; // Fecha o diálogo
    }
  }

}
</script>

<style></style>
