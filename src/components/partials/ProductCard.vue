<script>
  export default {
    props: {
      // ProductCard
    },
    data (){
      return {
        // products
      }
    }
  }
</script>



<template>

    <div class="product">

      <img id="immagine" src="./img/1.webp" alt="1.webp">
      <img id="immagine-hover" src="./img/1b.webp" alt="1b.webp">
      <div class="heart"><span>&hearts;</span></div>

      <div class="discount"><strong>-50%</strong></div>
      <div class="eco"><strong>Sostenibilità</strong></div>

      <div class="testo">
        <figcaption>Levi's</figcaption>
        <h4>RELAXED FIT TEE UNISEX</h4>
        <span class="costo" ><strong>14,99 &euro;</strong></span>
        <span class="ex-costo" >29,99 &euro;</span>
      </div>
      

  </div>
</template>



<style lang="scss" scoped>
@use '../../assets/scss/partials/general' as *;
@use '../../assets/scss/partials/variables' as *;
  
.product {
  width: 440px;
  height: 450px;
  margin: 150px 5px;
  position: relative;
}

#immagine{
  width: 440px;
  height: 640px;
  
}


#immagine-hover{
  width: 440px;
  height: 640px;
  position: absolute;
  top: 0;
  left: 0;
  z-index: -1;
}



#immagine:hover{
  opacity: 0;
}


.product .heart {
  font-size: 2rem;
  position: absolute;
  top: 5px;
  right: 0px;
  background-color: white;
  padding: 5px 5px;
}

.product .discount  {
  position: absolute;
  bottom: -160px;
  left: 0px;
  background-color: red;
  padding: 4px 8px;
  font-size: 10px;
  color: white;
}

.eco  {
  position: absolute;
  bottom: -160px;
  left: 45px;
  background-color: green;
  padding: 2px 8px;
  font-size: 12px;
  color: white;
}

.eco-p {
  position: absolute;
  bottom: -160px;
  left: 0px;
  background-color: green;
  padding: 2px 8px;
  font-size: 12px;
  color: white;
}

.testo{
  line-height: 1.1;
  font-size: 14px;
}

.testo figcaption{
  color: rgb(157, 134, 96);

}

.costo{
  color: red;
  text-decoration: bold;
}

.ex-costo{
  text-decoration: line-through;
}

</style>