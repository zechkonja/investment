<template>
  <div class="footer" id="contact">
    <div class="col-xs-12">
        <div class="box">
          <div class="row center-xs center-sm center-md center-lg">
              <div class="col-xs-12 col-sm-12 col-md-12 col-lg-12 footer-content">
                <img class="logo-img" src="../assets/images/logo.png" />
              </div>
              <div class="col-xs-12 col-sm-9 col-md-9 col-lg-9 footer-content">
                <div>
                  <p>Fusce felis eros, luctus eu tempus nec, auctor at nisl.
                    Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas.
                    Vivamus blandit nisi cursus nulla dapibus ut vehicula neque interdum.
                  </p>
                </div>
              </div>
              <div class="col-xs-10 col-sm-4 col-md-4 col-lg-4">
                <div class="footer-social-media">
                  <a href="#"><img src="../assets/images/twitter.png" /></a>
                  <a href="#"><img src="../assets/images/facebook.png" /></a>
                  <a href="#"><img src="../assets/images/linkedin.png" /></a>
                  <a href="#"><img src="../assets/images/dribble.png" /></a>
                  <a href="#"><img src="../assets/images/pinterest.png" /></a>
                  <a href="#"><img src="../assets/images/tumblr.png" /></a>
                  <a href="#"><img src="../assets/images/behance.png" /></a>
                  <a href="#"><img src="../assets/images/vimeo.png" /></a>
                </div>
              </div>
          </div>
        </div>
    </div>
    <div class="col-xs-12">
        <div class="box">
          <div class="row center-xs center-sm center-md center-lg">
              <div class="col-xs-12 col-sm-12 col-md-12 col-lg-12 footer-bottom">
                <ul>
                  <li><a href="#">Legal</a></li>
                  <li><a href="#">Privacy</a></li>
                  <li><a href="#">Contact</a></li>
                </ul>
              </div>
          </div>
        </div>
    </div>
</div>

  </div>
</template>

<script>

export default {
  name: 'Footer',
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
    color: white;
  }

  .footer{
    background-color: #222222;
  }

  .footer-content img{
    margin-top: 20px;
  }

  .footer-content p{
    font-size: 14px;
  }

  .logo-img{
    margin: 0 auto;
    width: auto;
    padding-top: 25px;
    padding-bottom: 20px;
  }

  .footer-social-media{
    max-width: 250px;
    border: 1px solid #434343;
    border-radius: 2px;
    margin: 15px auto 40px auto;
  }

  .footer-social-media a {
    display: inline-block;
    padding: 5px;
  }

  .footer-social-media img{
    width: auto;
    height: auto;
  }

  .footer-bottom{
    background-color: #1f1f1f;
  }

  .footer-bottom ul {
    padding-left: 0;
  }

  .footer-bottom ul li {
      display: inline-block;
  }

  .footer-bottom ul li a {
    font-family: 'MyriadPro';
    font-weight: 100;
    color: white;
    font-size: 13px;
    opacity: 0.6;
    padding-left: 5px;
    padding-right: 5px;
  }

  .footer-bottom ul li a {
    text-decoration: none;
  }


</style>
