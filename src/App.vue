<template>
  <div>
    <app-header v-bind:title="title" v-on:changeTitle= "updateTitle"></app-Header>
    <app-ninjas v-bind:ninjas="ninjas"></app-ninjas>
    <app-todo>
    <div slot="form-header">
    <h3>This is the title of a form</h3>
    <p>This is some info about the form</p>
</div>
<div slot="form-fields">
    <input type="text" placeholder="name" required />
    <input type="password" placeholder="password" required />
</div>
<div slot="form-controls">
    <button v-on:click="handleSubmit">Submit</button>
</div>

    </app-todo>
    <lobsang></lobsang>

    <app-footer></app-footer>
  </div>
</template>

<script>
import  Header from './component/Header.vue';
import  Ninjas from './component/Ninjas.vue';
import  Footer from './component/Footer.vue';
import  Todo from './component/todo.vue';
import  Lobsang from './component/lobsang.vue';

export default {
components:{
'app-header': Header,
'app-ninjas': Ninjas,
'app-footer': Footer,
'app-todo'  : Todo,
'lobsang'   : Lobsang
},
  data () {
    return {
      title: "  ninja App",
      ninjas:[
      {name:"lobsang",sex:"male",age:23,show:false},
      {name:"gyatso",sex:"male",age:22,show:true},
      {name:"tenzin",sex:"girl",age:24,show:false},


      ]
    }
  },
  methods:{
    updateTitle:function(data){
      this.title=data;
},

  handleSubmit: function(){
      alert('thanks for submitting');

}
  }
}
</script>

<style scoped>

</style>
