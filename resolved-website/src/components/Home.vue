<template>
   <section id="home" data-parallax="scroll" data-image-src="../assets/images/hero-bg.jpg" data-natural-width="3000" data-natural-height="2000">
        <div class="overlay"></div>
        <div class="home-content">        

            <div class="row contents">                     
                <div class="home-content-left">

                    <h3 data-aos="fade-up" class="aos-init aos-animate">Welcome to Dazzle</h3>

                    <h1 data-aos="fade-up" class="aos-init aos-animate">
                        Creative Landing <br>
                        Page to Showcase <br>
                        Your Amazing App.
                    </h1>

                    <div class="buttons aos-init aos-animate" data-aos="fade-up">
                        <a href="#download" class="smoothscroll button stroke">
                            <i class="fa fa-arrow-circle-down"></i>
                            Download App
                        </a>
                        <a href="http://player.vimeo.com/video/14592941?title=0&amp;byline=0&amp;portrait=0&amp;color=39b54a" data-lity="" class="button stroke">
                            <i class="fa fa-play"></i>
                            Watch Video
                        </a>
                    </div>                                         

                </div>

                <div class="home-image-right">
                    <img src="../assets/images/iphone-app-470.png" srcset="../assets/images/iphone-app-470.png 1x, ../assets/images/iphone-app-940.png 2x" data-aos="fade-up" class="aos-init aos-animate">
                </div>
            </div>

        </div> <!-- end home-content -->

        <ul class="home-social-list">
            <li>
                <a href="#"><i class="fa fa-facebook-square"></i></a>
            </li>
            <li>
                <a href="#"><i class="fa fa-twitter"></i></a>
            </li>
            <li>
                <a href="#"><i class="fa fa-instagram"></i></a>
            </li>
            <li>
                <a href="#"><i class="fa fa-youtube-play"></i></a>
            </li>
        </ul>
        <!-- end home-social-list -->

        <div class="home-scrolldown">
            <a href="#about" class="scroll-icon smoothscroll">
                <span>Scroll Down</span>
                <i class="fa fa-chevron-right" aria-hidden="true"></i>
            </a>
        </div>

    </section> <!-- end home -->  
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Home extends Vue {
  @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

/* ===================================================================
 *  10. home - (_site-layout.scss)
 *
 * ------------------------------------------------------------------- */

#home {
  width: 100%;
  height: 786px;
  min-height: 786px;
  background-color: transparent;
  position: relative;
  display: table;
}

#home .shadow-overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  opacity: 0.2;
  background: -moz-linear-gradient(left, black 0%, black 20%, transparent 100%);
  /* FF3.6-15 */
  background: -webkit-linear-gradient(
    left,
    black 0%,
    black 20%,
    transparent 100%
  );
  /* Chrome10-25,Safari5.1-6 */
  background: linear-gradient(to right, black 0%, black 20%, transparent 100%);
  /* W3C, IE10+, FF16+, Chrome26+, Opera12+, Safari7+ */
  filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#000000', endColorstr='#00000000', GradientType=1);
  /* IE6-9 */
}
#home .overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  opacity: 0.2;
  background-color: #000000;
}
.no-js #home {
  background: #151515;
}
.home-content {
  display: table-cell;
  width: 100%;
  height: 100%;
  vertical-align: bottom;
}
.home-content .contents {
  position: relative;
}
.home-content-left {
  padding: 15rem 0 12rem 40px;
  position: relative;
  width: 50%;
}
.home-content-left h3 {
  color: rgba(255, 255, 255, 0.8);
  font-size: 1.6rem;
  line-height: 1.5;
  text-transform: uppercase;
  letter-spacing: 0.2rem;
  margin-bottom: 2.4rem;
}
.home-content-left h1 {
  font-family: "Montserrat", sans-serif;
  font-size: 5.2rem;
  letter-spacing: -0.05rem;
  line-height: 1.269;
  color: #ffffff;
  margin-bottom: 9rem;
}
.home-content-left .button.stroke {
  color: #ffffff !important;
  border-color: #ffffff;
  margin: 0 0.6rem 1.2rem;
  padding: 0 2.2rem;
  min-width: 188px;
}
.home-content-left .button.stroke span[class*="icon"] {
  margin-right: 5px;
  position: relative;
  top: 2px;
}
.home-content-left .button.stroke:hover,
.home-content-left .button.stroke:focus {
  background-color: white !important;
  color: #000000 !important;
}
.home-image-right {
  display: block;
  position: absolute;
  right: 0;
  top: 50%;
  -webkit-transform: translateY(-50%);
  -ms-transform: translateY(-50%);
  transform: translateY(-50%);
  padding-top: 21rem;
  z-index: 500;
  width: 50%;
  text-align: right;
}
.home-image-right img {
  vertical-align: bottom;
  width: 75%;
}
/* home social-list */
.home-social-list {
  position: absolute;
  right: 42px;
  top: 50%;
  margin: 0;
  padding: 0;
  list-style: none;
  font-size: 2.2rem;
  line-height: 1.75;
  text-align: center;
  -webkit-transform: translateY(-55%);
  -ms-transform: translateY(-55%);
  transform: translateY(-55%);
}
.home-social-list::before {
  display: block;
  content: "";
  width: 2px;
  height: 42px;
  background-color: rgba(255, 255, 255, 0.15);
  margin-left: auto;
  margin-right: auto;
  margin-bottom: 12px;
}
.home-social-list li {
  padding-left: 0;
}
.home-social-list li a,
.home-social-list li a:visited {
  color: #ffffff;
}
.home-social-list li a:hover,
.home-social-list li a:focus,
.home-social-list li a:active {
  color: #44c455;
}
/* scroll down */
.home-scrolldown {
  position: absolute;
  bottom: 0;
  right: 0;
  -webkit-transform: rotate(90deg);
  -ms-transform: rotate(90deg);
  transform: rotate(90deg);
  -webkit-transform-origin: right top;
  -ms-transform-origin: right top;
  transform-origin: right top;
  float: right;
}
.home-scrolldown i {
  padding-left: 9px;
}
.home-scrolldown a:hover,
.home-scrolldown a:focus {
  color: #44c455 !important;
}
html[data-useragent*="MSIE 10.0"] .home-scrolldown,
.oldie .home-scrolldown {
  display: none;
}
.scroll-icon {
  display: inline-block;
  font-family: "Montserrat", sans-serif;
  font-weight: 620;
  font-size: 1.2rem;
  text-transform: uppercase;
  letter-spacing: 0.3rem;
  color: #ffffff !important;
  background: transparent;
  position: relative;
  top: 36px;
  right: 42px;
  -webkit-animation: animate-it 3s ease infinite;
  animation: animate-it 3s ease infinite;
}
.scroll-icon i {
  font-size: 2.4rem;
  position: relative;
  bottom: -6px;
}
/* vertical animation */
@-webkit-keyframes animate-it {
  0%,
  60%,
  80%,
  100% {
    -webkit-transform: translateX(0);
  }
  0%,
  60%,
  80%,
  100% {
    transform: translateX(0);
  }
  20% {
    -webkit-transform: translateX(-5px);
  }
  20% {
    transform: translateX(-5px);
  }
  40% {
    -webkit-transform: translateX(20px);
  }
  40% {
    transform: translateX(20px);
  }
}
@keyframes animate-it {
  0%,
  60%,
  80%,
  100% {
    -webkit-transform: translateX(0);
  }
  0%,
  60%,
  80%,
  100% {
    transform: translateX(0);
  }
  20% {
    -webkit-transform: translateX(-5px);
  }
  20% {
    transform: translateX(-5px);
  }
  40% {
    -webkit-transform: translateX(20px);
  }
  40% {
    transform: translateX(20px);
  }
}
/* ------------------------------------------------------------------- 
 * responsive:
 * home section 
 * ------------------------------------------------------------------- */
@media only screen and (max-width: 1300px) {
  .home-image-right {
    right: 5rem;
  }
}
@media only screen and (max-width: 1200px) {
  #home {
    overflow: hidden;
  }
  .home-content {
    vertical-align: middle;
  }
  .home-content-left {
    padding: 18rem 0 12rem 40px;
  }
  .home-content-left h3 {
    font-size: 1.5rem;
  }
  .home-content-left h1 {
    font-size: 4.8rem;
  }
  .home-image-right {
    padding-top: 18rem;
  }
  .home-image-right img {
    vertical-align: top;
    width: 70%;
  }
}
@media only screen and (max-width: 1100px) {
  .home-content-left h1 {
    font-size: 4.6rem;
  }
  .home-content-left h1 br {
    display: none;
  }
}
@media only screen and (max-width: 1024px) {
  .home-content-left {
    width: 60%;
    padding: 18rem 6rem 12rem 4rem;
  }
  .home-content-left h3 {
    font-size: 1.5rem;
  }
  .home-content-left h1 {
    font-size: 4.2rem;
  }
  .home-image-right {
    width: 40%;
    padding-top: 120px;
  }
  .home-image-right img {
    vertical-align: top;
    width: 100%;
  }
}
@media only screen and (max-width: 900px) {
  #home {
    height: auto;
    min-height: 840px;
  }
  #home,
  .home-content {
    display: block;
    text-align: center;
  }
  .home-content-left {
    width: 94%;
    position: static;
    padding: 15rem 6rem 366px;
    margin: 0 auto;
  }
  .home-content-left h1 {
    margin-bottom: 3.6rem;
  }
  .home-image-right {
    width: 400px;
    right: auto;
    top: auto;
    left: 50%;
    bottom: 0;
    -webkit-transform: translateX(-50%);
    -ms-transform: translateX(-50%);
    transform: translateX(-50%);
    padding: 0;
    margin-bottom: -378px;
  }
}
@media only screen and (max-width: 768px) {
  #home {
    min-height: auto;
  }
  .home-content-left h3 {
    font-size: 1.4rem;
  }
  .home-content-left h1 {
    font-size: 3.6rem;
  }
}
@media only screen and (max-width: 600px) {
  .home-content-left {
    padding: 12rem 6rem 366px;
  }
  .home-content-left h1 {
    font-size: 3.3rem;
  }
  .home-content-left .button.stroke {
    width: 100%;
    min-width: 0;
    max-width: 280px;
  }
  .home-social-list {
    font-size: 2rem;
    right: 30px;
  }
  .scroll-icon {
    top: 21px;
  }
}
@media only screen and (max-width: 500px) {
  .home-social-list,
  .home-scrolldown {
    display: none;
  }
  .home-content-left {
    padding: 12rem 2.5rem 366px;
    width: 100%;
  }
  .home-content-left h1 {
    font-size: 3rem;
  }
}
@media only screen and (max-width: 400px) {
  .home-content-left {
    padding: 12rem 0 300px;
  }
  .home-content-left .button.stroke {
    margin: 0 0 1.2rem 0;
  }
  .home-image-right {
    width: 320px;
    margin-bottom: -298px;
  }
}
</style>
