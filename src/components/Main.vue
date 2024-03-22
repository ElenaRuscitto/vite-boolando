<script>
import ProductCard from './partials/ProductCard.vue';
  export default {

    components: {
      ProductCard
    },
    
    data(){
      return {

      }
    }
  }

</script>



<template>

  <main>
    <div class="container">

      <ProductCard />

    </div>
    
  </main>

</template>




<style lang="scss" scoped>
@use '../assets/scss/partials/general';
@use '../assets/scss/partials/variables' as *;

.container {
  padding-top: 100px;
}

.container {
	display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
}
</style>