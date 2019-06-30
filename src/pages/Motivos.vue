<template>

  <div class="q-pa-md">

    <div class="row">
      <div class="col text-center">
        <h4>O que motivou sua insatisfação?</h4>
      </div>
    </div>

    <div class="row motivo text-center" v-for="motivo in motivos" :key="motivo">
        <div class="col-md-4 col-sm-3 col-xs-2"></div>
        <div class="col-md col-sm col-xs">
            <q-btn class="full-width" color="secondary" :label="motivo" @click="goPage('concluido')" />
        </div>
        <div class="col-md-4 col-sm-3 col-xs-2"></div>
    </div>

  </div>
</template>

<style>
</style>

<script>
export default {
  name: 'Motivos',
  data () {
    return {
      motivos: [
        'Velocidade no atendimento',
        'Falta de educação',
        'Outros'
      ]
    }
  },
  methods: {
    goPage (rota) {
      this.$router.replace(`/${rota}`)
    }
  }
}
</script>

<style scoped>
.motivo{
    margin-top: 1%;
}
</style>
