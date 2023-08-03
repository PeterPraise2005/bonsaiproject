<template>
  <div class="container">
          <form method="Get">
          <h1>Register</h1>
          <input required type="text" class="form-control" v-model="name" placeholder="Enter Your UserName"><br>
          <button id="post" class="btn btn-success" type="submit">Register</button>
         </form>
  </div>
</template>

<script>
export default {
    name:'RegisterView',
     }

</script>

<style>

</style>