<template>
  <div class="container mt-5">
      <form method="get">
          <h1>Log In</h1>
          <input required type="text" class="form-control" placeholder="UserName"><br>
          <button class="btn btn-primary" type="submit">Log In</button>
      </form>
  </div>
   <RegisterView />
</template>

<script>
import RegisterView from '@/views/RegisterView.vue'
export default {
    name:'LogView',
    components:{
        RegisterView
    },
}
</script>

<style scoped>
*{
    background-color: rosybrown;
}
</style>