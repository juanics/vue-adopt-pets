<template>
  <div>
    <h1>Dogs for Adoption</h1>
    <b-table bordered hover striped :items="dogs"></b-table>
  </div>
</template>

<script>
import dogs from '@/data/dogs.js'
export default {
  data () {
    return {
      name: 'Dogs',
      dogs: dogs
    }
  }
}
</script>

<style>

</style>
