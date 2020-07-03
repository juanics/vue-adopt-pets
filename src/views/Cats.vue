<template>
  <div>
    <h1>Cats for Adoption</h1>
    <b-table bordered striped hover :items="cats"></b-table>
  </div>
</template>

<script>
import cats from '@/data/cats.js'

export default {
  data () {
    return {
      cats: cats
    }
  }
}
</script>

<style>

</style>
