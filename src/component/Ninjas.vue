<template>
    <div id="ninjas">
    <input type="text" v-model="name">{{name}}
      <ul>
        <li v-for="ninja in ninjas"  v-on:click="ninja.show =!ninja.show">
          <h2>{{ninja.name}}
          </h2>
          <h3 v-show="ninja.show">{{ninja.sex}}</h3>
          </li>
      </ul>
    </div>

</template>
<script>
  export default{
  props:['ninjas'],
    data(){
      return{

      name:''
      }
    },

  }
</script>

<style scoped>


<style>
