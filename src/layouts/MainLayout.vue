<template>
  <q-layout view="lHh Lpr lFf" class="">
    <q-header elevated>
      <q-toolbar class="bg-accent">
        <q-btn flat dense round icon="menu" aria-label="Menu" @click="toggleLeftDrawer" />

        <q-toolbar-title>
          <!-- Quasar App -->
        </q-toolbar-title>

        <!-- <div>Quasar v{{ $q.version }}</div> -->
      </q-toolbar>
    </q-header>

    <q-drawer v-model="leftDrawerOpen" show-if-above bordered>
      <q-list>
        <q-item-label header>
          Menu
        </q-item-label>

        <EssentialLink v-for="link in essentialLinks" :key="link.titulo" v-bind="link" />
      </q-list>
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import { defineComponent, ref } from 'vue'
import EssentialLink from 'components/EssentialLink.vue'

const linksList = [
  {
    titulo: 'Pagina Inicial',
    caption: 'Informações Gerais',
    icon: 'school',
    rota: '/'
  },
  {
    titulo: 'Jogo Tarot',
    caption: 'Escolher as cartas que refletem a sorte',
    icon: 'chat',
    rota: 'jogoTarot'
  },
  {
    titulo: 'Cartas Tarot',
    caption: 'Info das cartas no Tarot',
    icon: 'code',
    rota: 'cartasTarot'
  }
]

export default defineComponent({
  name: 'MainLayout',

  components: {
    EssentialLink
  },

  setup() {
    const leftDrawerOpen = ref(false)

    return {
      essentialLinks: linksList,
      leftDrawerOpen,
      toggleLeftDrawer() {
        leftDrawerOpen.value = !leftDrawerOpen.value
      }
    }
  }
})
</script>
