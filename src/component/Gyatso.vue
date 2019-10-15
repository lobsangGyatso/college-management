<template>
  <div>
  <slot name="header" v-bind:user="user"></slot>
  </div>
</template>

<script>


export default {

    data () {
        return {
          user:[
          {name:'lobsang',age:23},
          {name:'gyatso',age:23},
          {name:'tenzin',age:22}
          ]
        }
    },
    methods: {
    }
}
</script>

<style scoped>

</style>
