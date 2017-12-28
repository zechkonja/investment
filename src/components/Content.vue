<template>
  <div class="content">
    <!-- FEATURES -->
    <section id="features">
      <div class="container">
        <div class="row center-xs center-sm center-md center-lg">
          <div class="col-xs-12 col-sm-12 col-md-12 col-lg-12">

            <div class="row center-xs center-sm center-md center-lg" id="why">
              <div class="col-xs-12 col-sm-4 col-md-4 col-lg-4 service-block platform">
                <div class="image-block">
                  <img class="platform-image" src="../assets/images/Platform.png" />
                </div>
                <h2>State Of The Art Platform</h2>
                <p>Vestibulum tincidunt placerat ligula sed vestibulum. Phasellus nec enim ac enim placerat ligula sed vestibulum</p>
              </div>
              <div class="col-xs-12 col-sm-4 col-md-4 col-lg-4 service-block network">
                <div class="image-block"><img class="platform-image" src="../assets/images/Network.png" /></div>
                <h2>Network Focused</h2>
                <p>Vestibulum tincidunt placerat ligula sed vestibulum. Phasellus nec enim ac enim placerat ligula sed vestibulum</p>
              </div>
              <div class="col-xs-12 col-sm-4 col-md-4 col-lg-4 service-block market">
                <div class="image-block"><img class="platform-image" src="../assets/images/Market-access.png" /></div>
                <h2>Access To Wider Private Market</h2>
                <p>Vestibulum tincidunt placerat ligula sed vestibulum. Phasellus nec enim ac enim placerat ligula sed vestibulum</p>
              </div>
            </div>
            <hr class="separator" />

            <div class="row center-xs center-sm center-md center-lg"  id="blog">
              <div class="col-xs-12 col-sm-12 col-md-12 col-lg-12 center-service">
                <h2>We serve leading networks across the private investment spectrum</h2>
                <p>Vestibulum tincidunt placerat ligula sed vestibulum. Phasellus nec enim ac enim congue tincidunt.
                   Curabitur molestie urna justo, quis varius urna convallis ac. Vestibulum nec dictum nulla.
                   Aenean consectetur non nulla ac tristique. Proin nibh dolor, rutrum et sollicitudin nec, semper at ipsum.</p>
              </div>
            </div>

            <div class="row center-xs center-sm center-md center-lg bottom-service">
              <div class="col-xs-12 col-sm-4 col-md-4 col-lg-4 ">
                <div class="image-content">
                  <img class="" src="../assets/images/pic1.jpg" />
                  <p class="caption">View details</p>
                </div>
                <h3 class="content-title">Financial Institutions</h3>
              </div>
              <div class="col-xs-12 col-sm-4 col-md-4 col-lg-4">
                <div class="image-content">
                  <img class="" src="../assets/images/pic2.jpg" />
                  <p class="caption">View details</p>
                </div>
                <h3 class="content-title">Innovation and Corporate Ventures</h3>
              </div>
              <div class="col-xs-12 col-sm-4 col-md-4 col-lg-4">
                <div class="image-content">
                  <img class="" src="../assets/images/pic3.jpg" />
                  <p class="caption">View details</p>
                </div>
                <h3 class="content-title">Investment Networks</h3>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>

export default {
  name: 'Content',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

  h2, p, h3 {
    font-family: 'MyriadPro';
    font-weight: 100;
  }

  h3 {
    opacity: 0.7;
  }

  p {
    opacity: 0.7;
    font-size: 12px;
  }



  .service-block{
    padding: 20px;
    margin-top: 40px;
    font-family: 'MyriadPro';
  }

  .image-block{
    position: relative;
    width: 110px;
    height:110px;
    border-radius: 5px;
    margin: auto;
  }

  .service-block {
    display: grid;
  }


  .service-block p {
    vertical-align: bottom;
  }

  .service-block h2 {
        word-spacing: 1px;
  }

  .platform .image-block{
    background: rgb(130,93,50); /* Old browsers */
    background: -moz-linear-gradient(left, rgba(130,93,50,1) 0%, rgba(136,96,49,1) 0%, rgba(109,106,66,1) 100%); /* FF3.6-15 */
    background: -webkit-linear-gradient(left, rgba(130,93,50,1) 0%,rgba(136,96,49,1) 0%,rgba(109,106,66,1) 100%); /* Chrome10-25,Safari5.1-6 */
    background: linear-gradient(to right, rgba(130,93,50,1) 0%,rgba(136,96,49,1) 0%,rgba(109,106,66,1) 100%); /* W3C, IE10+, FF16+, Chrome26+, Opera12+, Safari7+ */
    filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#825d32', endColorstr='#6d6a42',GradientType=1 ); /* IE6-9 */
  }

  .network .image-block{
    background: rgb(130,93,50); /* Old browsers */
    background: -moz-linear-gradient(left, rgba(130,93,50,1) 0%, rgba(27,155,190,1) 0%, rgba(23,98,136,1) 100%); /* FF3.6-15 */
    background: -webkit-linear-gradient(left, rgba(130,93,50,1) 0%,rgba(27,155,190,1) 0%,rgba(23,98,136,1) 100%); /* Chrome10-25,Safari5.1-6 */
    background: linear-gradient(to right, rgba(130,93,50,1) 0%,rgba(27,155,190,1) 0%,rgba(23,98,136,1) 100%); /* W3C, IE10+, FF16+, Chrome26+, Opera12+, Safari7+ */
    filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#825d32', endColorstr='#176288',GradientType=1 ); /* IE6-9 */
  }

  .market .image-block{
    background: rgb(130,93,50); /* Old browsers */
    background: -moz-linear-gradient(left, rgba(130,93,50,1) 0%, rgba(99,46,39,1) 0%, rgba(97,52,44,1) 100%); /* FF3.6-15 */
    background: -webkit-linear-gradient(left, rgba(130,93,50,1) 0%,rgba(99,46,39,1) 0%,rgba(97,52,44,1) 100%); /* Chrome10-25,Safari5.1-6 */
    background: linear-gradient(to right, rgba(130,93,50,1) 0%,rgba(99,46,39,1) 0%,rgba(97,52,44,1) 100%); /* W3C, IE10+, FF16+, Chrome26+, Opera12+, Safari7+ */
    filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#825d32', endColorstr='#61342c',GradientType=1 ); /* IE6-9 */
  }

  .platform-image{
    width: auto;
    height: auto;
    padding: 20px;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);

  }

  .center-service p{
    font-size: 14px;
  }

  .image-content{
    max-width: 100%;
    max-height: 100%;
    position: relative;
    display: inline-block;
  }

  .image-content img {
    position: relative;
    float: left;
    width:  100%;
    height: 250px;
    background-position: 50% 50%;
    background-repeat:   no-repeat;
    background-size:     cover;
  }

  .image-content .caption {
    position:relative;
    left:0px;
    visibility:hidden;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    background-color: #ee7421;
    padding: 5px 20px;
    color: white;
  }

  .image-content:hover {
    background-color: #ee7421;
  }

  .image-content:hover img {
    opacity: 0.7;
    cursor: pointer;
  }

  .image-content:hover p {
    opacity: 1;
  }


  .image-content:hover .caption {
    visibility:visible;
  }

  .separator{
    opacity: 0.5;
  }


  .center-service{
    margin-bottom: 35px;
  }

  .center-service h2 {
    margin-top: 45px;
  }

  .center-service p {
    text-align: center;
    word-break: break-all;
    padding: 15px;
    opacity: 0.5;
  }

  .content-title{
    margin-top: 5px;
  }

  .bottom-service {
    margin-bottom: 50px;
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
      .image-content{
        margin-left: 15px;
        margin-right: 15px;
      }
      .center-service h2 {
        margin-left: 5px;
        margin-right: 5px;
      }
  }

  @media (max-width:320px)  {

  }


</style>
