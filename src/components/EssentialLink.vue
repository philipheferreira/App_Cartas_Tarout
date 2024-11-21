<template>
  <q-item clickable :to="rota">
    <q-item-section v-if="icon" avatar>
      <q-icon :name="icon" />
    </q-item-section>

    <q-item-section>
      <q-item-label>{{ titulo }}</q-item-label>
      <q-item-label caption>{{ descricao }}</q-item-label>
    </q-item-section>
  </q-item>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'EssentialLink',
  props: {
    titulo: {
      type: String,
      required: true
    },

    descricao: {
      type: String,
      default: ''
    },

    rota: {
      type: String,
      default: '#'
    },

    icon: {
      type: String,
      default: ''
    }
  }
})
</script>
