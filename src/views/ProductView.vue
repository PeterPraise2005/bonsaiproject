<template>
  <div class="container">
      <!-- <p v-if="Pleasewait">Please Wait.....</p> -->
      <h4>Product {{ $route.params.id}}</h4>
  </div>
</template>

<script setup>
    import { ref, onMounted } from 'vue'; 
    import { useRoute } from 'vue-router';

    const Product = ref([])
    const  PleaseWait = ref(false)
    const route = useRoute()

    onMounted(async() =>{
        const result = await fetch(`https://tbhpwebdevapi.azurewebsites.net/api/BonsaiV2/${route.params.id}`)
        const response = await result.json();
        console.log(response)
        Product.value = response;
        PleaseWait.value = true

    })
</script>

<style>

</style>