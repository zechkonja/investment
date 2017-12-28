<template>
  <div class="header container-menu">
    <div class="row center-xs center-sm">
        <div class="col-xs-12 col-sm-8">
            <div class="box">
              <div class="row end-sm end-md end-lg">
                  <div class="col-xs-12 col-sm-2 col-md-2 col-lg-2">
                    <a href="#app" @click="setCurrentHome()" v-smooth-scroll><img class="logo-img" src="../assets/images/logo.png" /></a>
                  </div>
                  <div class="col-xs-12 col-sm-10 col-md-10 col-lg-10">
                    <nav id="navbar">
                      <ul>
                        <li class="current" ref="app"><a href="#app" @click="setCurrent($event)" v-smooth-scroll>Home</a></li>
                        <li><a href="#why" @click="setCurrent($event)" v-smooth-scroll="{ duration: 2000 }">Why</a></li>
                        <li><a href="#blog" @click="setCurrent($event)" v-smooth-scroll="{ duration: 2000 }">Blog</a></li>
                        <li><a href="#contact" @click="setCurrent($event)" v-smooth-scroll="{ duration: 2000 }">Contact</a></li>
                      </ul>
                    </nav>
                  </div>
              </div>
            </div>
        </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'Header',
  data: function(){
    return{
      activeClass: ''
    }
  },
  ready: function () {

  },
  methods: {
    setCurrent: function(event){
      let element = event.target.parentElement;
      this.removeCurrentSiblings(element);
      element.classList.add('current');
    },
    setCurrentHome: function(){
      let element = this.$refs.app;
      this.removeCurrentSiblings(element);
      element.classList.add('current');
    },
    removeCurrentSiblings: function (elem) {
        var siblings = [];
        var sibling = elem.parentNode.firstChild;
        var skipMe = elem;
        for ( ; sibling; sibling = sibling.nextSibling )
           if ( sibling.nodeType == 1 && sibling != elem ){
              sibling.classList.remove('current');
              siblings.push( sibling );
            }
        return siblings;
    }

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

  .container-menu {
   position: fixed;
   width: 100%;
   opacity: 0.7;
   z-index: 1;
   top: 0;
   left: 0;

   /* Permalink - use to edit and share this gradient: http://colorzilla.com/gradient-editor/#000000+0,000000+100&1+57,0.65+79,0.65+79,0.65+79,0.65+79,0+100 */
 background: -moz-linear-gradient(left, rgba(0,0,0,1) 0%, rgba(0,0,0,1) 57%, rgba(0,0,0,0.65) 79%, rgba(0,0,0,0) 100%); /* FF3.6-15 */
 background: -webkit-linear-gradient(left, rgba(0,0,0,1) 0%,rgba(0,0,0,1) 57%,rgba(0,0,0,0.65) 79%,rgba(0,0,0,0) 100%); /* Chrome10-25,Safari5.1-6 */
 background: linear-gradient(to right, rgba(0,0,0,1) 0%,rgba(0,0,0,1) 57%,rgba(0,0,0,0.65) 79%,rgba(0,0,0,0) 100%); /* W3C, IE10+, FF16+, Chrome26+, Opera12+, Safari7+ */
 filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#000000', endColorstr='#00000000',GradientType=1 ); /* IE6-9 */

  }

  .logo-img{
    margin: 0 auto;
    width: auto;
    padding-top: 25px;
    padding-bottom: 20px;
  }

  /* NAVBAR */
  #navbar{
    text-transform:uppercase;
    height: 100%;
  }

  #navbar ul{
    height: 100%;
    margin: 0;
  }

  #navbar li{
    display:inline-block;
    text-align: center;
    list-style:none;
    height: 98%;
    padding-left: 10px;
    padding-right: 10px;
    display: inline-flex;
    justify-content: center;
    align-items: center;
  }

  #navbar a{
    font-size: 12px;
    text-decoration:none;
    color:#888;
  }

  #navbar li.current, #navbar li:hover{
    color:#56a79a;
    border-bottom: 3px solid #dd3f19;
  }

  @media (max-width:1281px) {

  }
  @media (max-width:1025px) {

  }

  @media (max-width:961px)
  {

  }

  @media (max-width:768px)  {

  }

  @media (max-width:641px)  {
  }

  @media (max-width:481px)  {

  }

  @media (max-width:320px)  {

  }



</style>
