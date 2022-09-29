<template>
 <MyNavbar :logo="logo_src" :alt="app_name"/>
  <router-view/>
  <Footer/>
</template>

<script>
import MyNavbar from './components/MyNavbar.vue';
import Footer from './components/Footer.vue';

export default {
  components: {
    MyNavbar,
    Footer
  },
  data(){
    return{
      logo_src: "/img/logo.png",
      app_name:"Faça o seu Burger"
    }
  }
}

</script>

<style>
  * {
    font-display: Helvetica;
    padding: 0;
    margin: 0;
    box-sizing: border-box;
  }
  .main-container {
    margin: 50px;
    min-height: 250px;
  }
  h1 {
    text-align: center;
    font-size: 42px;
    margin-bottom: 30px;
    color: #222;
  }
</style>
