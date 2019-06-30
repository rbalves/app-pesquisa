<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>
      <q-toolbar>
        <q-btn
          flat
          dense
          round
          aria-label="Menu"
        >
          <q-icon name="search" />
        </q-btn>

        <q-toolbar-title>
          Pesquisa de atendimento
        </q-toolbar-title>

      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>

export default {
  name: 'MyLayout',
  data () {
    return {

    }
  },
  methods: {

  }
}
</script>

<style>
</style>
