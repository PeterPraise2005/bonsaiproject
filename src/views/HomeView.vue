<template>
  <div class="home">
        <h1>Welcome To group One Bonsai Tree Projects</h1>
      <h4>Motto::Bring Our Best To Your Door Steps</h4>
  </div>
   <h2>Indoor Bonsai's</h2>
    <div class="d-flex">
   <div class="card" style="width: 20rem;">
         <img src="../assets/images/ini1.png" class="card-img-top" alt="...">
          <div class="card-body">
           <h5 class="card-title">Card title</h5>
           <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
  </div>
</div>
   <div class="card" style="width: 20rem;">
         <img src="../assets/images/ini2.png" class="card-img-top" alt="...">
          <div class="card-body">
           <h5 class="card-title">Card title</h5>
           <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
  </div>
</div>
   <div class="card" style="width: 20rem;">
         <img src="../assets/images/ini3.png" class="card-img-top" alt="...">
          <div class="card-body">
           <h5 class="card-title">Card title</h5>
           <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
  </div>
</div>
    </div>

    <h2>Outdoor Bonsai's</h2>
    <div class="d-flex">
       <div class="card" style="width: 20rem;">
         <img src="../assets/images/out1.png" class="card-img-top" alt="...">
          <div class="card-body">
           <h5 class="card-title">Card title</h5>
           <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
  </div>
    </div>
       <div class="card" style="width: 20rem;">
         <img src="../assets/images/out2.png" class="card-img-top" alt="...">
          <div class="card-body">
           <h5 class="card-title">Card title</h5>
           <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
  </div>
       </div>
       <div class="card" style="width: 20rem;">
         <img src="../assets/images/out3.png" class="card-img-top" alt="...">
          <div class="card-body">
           <h5 class="card-title">Card title</h5>
           <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
  </div>
       </div>
   </div>
   <h2>Bonsai Care</h2>
   <div class="d-flex">
      <div class="card" style="width: 20rem;">
         <img src="../assets/images/care1.png" class="card-img-top" alt="...">
          <div class="card-body">
           <h5 class="card-title">Card title</h5>
           <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
  </div>
       </div>
       <div class="card" style="width: 20rem;">
         <img src="../assets/images/care2.png" class="card-img-top" alt="...">
          <div class="card-body">
           <h5 class="card-title">Card title</h5>
           <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
  </div>
       </div>
       <div class="card" style="width: 20rem;">
         <img src="../assets/images/care3.png" class="card-img-top" alt="...">
          <div class="card-body">
           <h5 class="card-title">Card title</h5>
           <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
           <a href="./CareView.vue"><ButtonClick msg="View More" class="btn btn-primary"/></a>
  </div>
       </div>
   </div>
</template>

<script>
import ButtonClick from '@/components/ClickComponent.vue'

export default {
  name: 'HomeView',
  components:{
    ButtonClick
  }
}

</script>

<style scoped>
.img-fluid{
  width: 3.5rem;
  
  
}
.image{
  width: 3.5rem;
}
.home{
  background-image: url(../assets/bgimg2.png);
  background-position: 50px;
  background-repeat: no-repeat;
  background-size: 100%;
}
h1{
  color: white;
}
h4{
  color: peachpuff;
}
.card{
  margin: 3.5rem;
}
</style>