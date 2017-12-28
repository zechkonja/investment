<template>
  <div class="container">
    <AppHeader />
    <AppSlider />
    <AppContent />
    <AppFooter />
    <vm-back-top :bottom="100" :duration="1000" :timing="'ease'">
     <div class="top"><img src="../assets/images/arrowUp.png" /></div>
   </vm-back-top>
  </div>
</template>

<script>
import AppHeader from '../components/Header'
import AppSlider from '../components/Slider'
import AppContent from '../components/Content'
import AppFooter from '../components/Footer'


export default {
  name: 'Container',
  components: {
    AppHeader, AppContent, AppFooter, AppSlider
  }
}
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

  @font-face {
      font-family: MyriadPro;
      src: url("../assets/fonts/MyriadPro-Regular.otf") format("opentype");
  }
  .container{
    margin:auto;
    width: 100%;
  }


  .top{
        padding: 20px;
        position: relative;
        background: rgba(17, 17, 17, .7);
        color: #fff;
        text-align: center;
        border-radius: 2px;
    }

    .top:hover{
          background: rgba(238,116,33, .7);
          color: #fff;
          text-align: center;
          border-radius: 2px;
      }

      .top img {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        width: auto;
        height: auto;
      }



</style>
