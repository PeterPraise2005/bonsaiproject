<template>
  <div class="container mt-5">
      <h3>Indoor Bonsai</h3>
      <h4>Indoor bonsai have become extremely popular in recent years. They make excellent gifts because they are different and say something about you. Most of them are tropical or semi-tropical species. They usually require lots of light and fairly constant temperature and humidity. The secret is not to forget to water them!</h4>
      <div class="row" v-for="product in products" :key="product.id">
          <div class="col-md-5 col-sm-3">
              <div class="card">
                  <div class="card-img-top"><img :src="product.productImage" alt="ProductImages"></div>
              </div>
              <div class="card-body">
                  <h5>{{ product.id }}</h5>
                  <h5>{{ product.productTitle }}</h5>
                  <h5>{{ product.productPrice }}</h5>
              </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name:'ProductView',
    data(){
        return{
            products:[],
            error:['']
        }
    },
    async mounted(){
        try{
            const result = await fetch('https://tbhpwebdevapi.azurewebsites.net/api/BonsaiV2/Category?category=indoor');
            const data = await result.json()
            console.log(data)
            this.products = data
        }catch(error){
            this.error = error
        }
    }
}
</script>

<style scoped>
    .img-centered-text{
        cursor: pointer;
    }
</style>