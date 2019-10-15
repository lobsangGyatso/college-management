<template>
<div>
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


</template>

<script>
export default{

  data(){
    return{

    }
  }


}
</script>

<style scoped>
</style>
