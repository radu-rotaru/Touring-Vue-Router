<template>
  <p>Regstration form here</p>
  <button @click="register">Register Me!</button>
</template>
<script>
export default {
  props: ['event'],
  methods: {
    register() {
      // If registration API call is successful
      // Push back to the event details
      // this.$router.push({
      //   name: 'EventDetails',
      //   params: { id: this.event.id }
      // } )
      this.$router.replace({ name: 'EventDetails', params: { id: 3 } })
    }
  }
}
</script>