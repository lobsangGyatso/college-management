<template>
  <footer>
  <p>{{copyright}}</p>
  </footer>
</template>

<script>
  export default{
      data(){
        return{
          copyright:  'Copyright 2019@gyatso '
        }
      }

  }

</script>

<style scoped>
footer{
background: black;
padding:10px;
},
p{
color: white;
text-align: center;
}
</style>
