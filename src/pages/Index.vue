<template>

  <div class="q-pa-md">

    <div class="row">
      <div class="col text-center">
        <h4>O que achou do nosso atendimento?</h4>
      </div>
    </div>

    <div class="row text-center">
      <div class="col"></div>
      <div class="col-xs-6 col-sm-3 col-md-3">
        <q-btn color="green" icon="thumb_up" label="Bom" @click="goPage('concluido')" />
      </div>
      <div class="col-xs-6 col-sm-3 col-md-3">
        <q-btn color="red" icon="thumb_down" label="Ruim" @click="goPage('motivos')" />
      </div>
      <div class="col"></div>
    </div>

  </div>
</template>

<style>
</style>

<script>
export default {
  name: 'PageIndex',
  methods: {
    goPage (rota) {
      this.$router.replace(`/${rota}`)
    }
  }
}
</script>
