<template>

  <div class="q-pa-md">

    <div class="row">
      <div class="col text-center">
        <h4>Obrigado por participar!</h4>
        <h5>Sua opinião é muito importante para nós!</h5>
      </div>
    </div>

  </div>
</template>

<style>
</style>

<script>
export default {
  name: 'Concluido',
  mounted () {
    setTimeout(() => this.$router.replace('/'), 4000)
  }
}
</script>
