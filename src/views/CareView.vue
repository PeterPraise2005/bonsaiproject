<template>
  <div>
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
    name:'CareView',

    data(){
        return{
            products:[],
            error:['']
        }
    },
    async mounted(){
        try{
            const result = await fetch('https://tbhpwebdevapi.azurewebsites.net/api/BonsaiV2/Category?category=care');
            const data = await result.json()
            console.log(data)
            this.products = data
        }catch(error){
            this.error = error
        }
    }
    // https://tbhpwebdevapi.azurewebsites.net/api/BonsaiV2/Category?category=care
}
</script>

<style>

</style>