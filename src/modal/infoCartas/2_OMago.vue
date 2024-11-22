<!-- ChildDialog.vue -->
<template>
  <q-dialog v-model="isOpen">
    <q-card style="max-width: 70%;" transition-show="rotate" transition-hide="rotate">
      <q-card-section>
        <div class="text-h6">II - O Mago</div>
      </q-card-section>
      <q-card-section>
        Este é um conteúdo vindo do componente filho.
      </q-card-section>
      <q-card-actions align="right">
        <q-btn flat label="Fechar" color="primary" @click="closeDialog" />
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
};
</script>
