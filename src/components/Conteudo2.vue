<template>
  <div>
      <input v-model="valor">
      <p v-if="quadrado % 2 == 0">{{ quadrado }}</p>
    <h3>Contato</h3>
    <p>Taciano</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      valor: 0
    }
  },
  computed: {
      quadrado() {
          return Math.pow(this.valor, 2)
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>