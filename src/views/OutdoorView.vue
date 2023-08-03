<template>
  <div>
      <h3>OutDoor Bonsai's</h3>
      <h4>As outdoor bonsai grow faster than indoor bonsai, you will see the results of reshaping, wiring and pruning much sooner. Outdoor bonsai also offer more scope for practising the hobby. Some enthusiasts make their own bonsai from garden and nursery plants, and some collect the raw material from the wild. You can also propagate your own plants from seed or cuttings or by layering. 
          <br> <br> Outdoor bonsai can be taken indoors from time to time. In fact, in countries such as China and Japan, it is traditional to use bonsai to decorate the home, but the trees are kept indoors for only short periods. After a day or two they are returned to their outdoor positions. The choice of outdoor bonsai is much wider than of indoor species.</h4>
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
    name:'OutdoorView',

    data(){
        return{
            products:[],
            error:['']
        }
    },
    async mounted(){
        try{
            const result = await fetch('https://tbhpwebdevapi.azurewebsites.net/api/BonsaiV2/Category?category=outdoor');
            const data = await result.json()
            console.log(data)
            this.products = data
        }catch(error){
            this.error = error
        }
    }
}
</script>

<style>

</style>