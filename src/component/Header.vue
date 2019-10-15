<template>
    <header>
    <h1 v-on:click="changeTitle">{{title}}</h1>
    </header>
</template>

<script>
export default{
props:['title'],
  data(){
      return{

        }
          },
          methods:{
            changeTitle:function(){
              this.$emit('changeTitle','lobsang title')
            }
          }
}
</script>

<style scoped>
header{
  background: lightgreen;
  padding:10px;
},
h1{
color: black;
text-align: center;
}
</style>
