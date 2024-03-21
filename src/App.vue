<script >
import Header from './Header.vue';
import Main from './Main.vue';
import Footer from './Footer.vue';

  export default {
    components: {
      Header,
      Main,
      Footer
    };

    data(){
      return {

      }
    }
  }

</script>



<template>

<Header />
<Main />
<Footer />

</template>




<style lang="scss" scoped>

  @use './assets/scss/main.scss';
  
</style>
