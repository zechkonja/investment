<template>
  <div class="slider">
    <div class="row center-xs center-sm">
        <div class="col-xs-12 col-sm-12">

          <div class="images" v-for="number in [currentNumber]" transition="fade">
            <img class="slider-image"
                 :src="images[Math.abs(currentNumber) % images.length]"
                 v-on:mouseover="stopRotation"
                 v-on:mouseout="startRotation"
                 />
              <div class="slider-caption">
                <h1>investment newtorks. connected</h1>
                <h3>We provide private platforms connecting professional investors to new opportunities,
                  in their organisation and other leading newtorks using our tech.
                </h3>
              </div>
              <div class="nav-dots">
                <label for="img-1" :class="{ checked: isActive(1) }" class="nav-dot" id="img-dot-1" @click="current(1)"></label>
                <label for="img-2" :class="{ checked: isActive(2) }" class="nav-dot" id="img-dot-2" @click="current(2)"></label>
                <label for="img-3" :class="{ checked: isActive(3) }" class="nav-dot" id="img-dot-3" @click="current(3)"></label>
              </div>
              <div class="left"><a @click="prev"><img src="../assets/images/leftArrow.png" /></a></div>
              <div class="right"><a @click="next"><img src="../assets/images/rightArrow.png" /></a></div>
          </div>

      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'AppSlider',
  data: function() {
    return {
      images: ['../src/assets/images/info-bg.jpg', '../src/assets/images/header-img.png', '../src/assets/images/info-bg.jpg'],
      currentNumber: 1,
      timer: null,
      activeClass: 'checked',
      numberOfSlides: 3
    }
  },

  ready: function () {
     this.startRotation();
  },

  methods: {
     startRotation: function() {
         this.timer = setInterval(this.next, 3000);
     },

     stopRotation: function() {
         clearTimeout(this.timer);
         this.timer = null;
     },

     next: function() {
         if(this.currentNumber < this.numberOfSlides){
           this.currentNumber += 1;
         } else {
           this.currentNumber = 1;
         }
     },
     prev: function() {
         if(this.currentNumber > 1){
           this.currentNumber -= 1;
         } else {
           this.currentNumber = this.numberOfSlides;
         }
     },
     current: function(number){
       this.currentNumber = number;
     },
     isActive: function(number){
       return this.currentNumber === number;
     }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

  .slider img {
    max-height: 100%;
    max-width: 100%;
  }

  .fade-transition {
    transition: all 0.8s ease;
    overflow: hidden;
    visibility: visible;
    opacity: 1;
    position: absolute;
  }
  .fade-enter, .fade-leave {
    opacity: 0;
    visibility: hidden;
  }

  .left {
    width: 65px;
    height: 115px;
    position: absolute;
    top: 50%;
    left: 5%;
  }

  .right {
    position: absolute;
    top: 50%;
    right: 5%;
  }

  .left:hover, .right:hover {
    cursor: pointer;
  }

  .images {
    position: relative;
  }

  .slider-caption {
    width: 43%;
    font-family: 'MyriadPro';
    line-height: 1;
    color: white;
    text-align: center;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }

  .slider-caption h1 {
    text-transform: uppercase;
    letter-spacing: 3px;
  }

  .slider-caption h3 {
      line-height: 1.7;
      opacity: 0.6;
  }

  .slider-caption h1, .slider-caption h3 {
    font-weight: 100;
  }

  .nav-dots {
  	width: 100%;
  	bottom: 25px;
  	height: 9px;
  	display: block;
  	position: absolute;
  	text-align: center;
  }

  .nav-dots .nav-dot {
  	top: -5px;
  	width: 7px;
  	height: 7px;
  	margin: 0 4px;
  	position: relative;
  	border-radius: 100%;
  	display: inline-block;
  	background-color: rgba(255,255,255, 0.6);
    border:1px solid transparent;
  }

  .nav-dots .nav-dot:hover {
  	cursor: pointer;
    background: rgba(255,255,255, 0);
    border:1px solid white;
  }

  .nav-dots .nav-dot.checked {
  	background: rgba(255,255,255, 0);
    border:1px solid white;
    width: 9px;
  	height: 9px;
  }



  @media (max-width:1281px) {

  }
  @media (max-width:1025px) {

  }

  @media (max-width:961px)
  {


    .slider-caption h1 {
      font-size: 20px;
    }

    .slider-caption h3 {
      font-size: 14px;
    }

    .left img, .right img{
      max-width: 60%;
      max-height: 60%;
    }

  }

  @media (max-width:768px)  {

  }

  @media (max-width:641px)  {

    .slider .images .slider-image {
      height: 450px;
    }

  }

  @media (max-width:481px)  {

  }

  @media (max-width:320px)  {

    .slider-caption {
      top: 55%;
    }

  }






</style>
