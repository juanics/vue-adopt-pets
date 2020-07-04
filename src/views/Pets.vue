<template>
  <div>
    <h1>{{animal.name}}</h1>
  </div>
</template>

<script>
import { mapState } from 'vuex'

export default {
  data () {
    return {
      animal: {},
      specie: ''
    }
  },
  computed: {
    ...mapState([
      'cats',
      'dogs'
    ])
  },
  mounted () {
    this.animal = this[this.$route.params.species][this.$route.params.id]
  },
  methods: {
    getSpecie () {
      this.specie = this.$route.params.species
    }
  }
}
</script>
