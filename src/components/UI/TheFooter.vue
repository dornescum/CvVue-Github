<template>
  <footer class="site-footer">
    <div class="container">
      <div class="row">
        <div class="col-md-8 col-sm-6 col-xs-12">
          <div class="d-flex" id="footer">
            <p class="pr-4">Linux fan</p>
            <a href="https://ubuntu.com/download/desktop" target="_blank" class="ubuntu">
              <i class="fab fa-ubuntu fa-2x"></i></a>
          </div>
        </div>
        <div class="col-md-4 col-sm-6 col-xs-12">
          <ul class="social-icons">
            <li><a class="github" href="https://github.com/dornescum.html" target="_blank"><i class="fab fa-github"></i></a></li>
            <li><a class="linkedin" href="https://www.linkedin.com/feed/" target="_blank"><i class="fab fa-linkedin"></i></a></li>

          </ul>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "TheFooter"
}
</script>

<style scoped>
.site-footer {
  background-color: #26272b;
  padding: 45px 0 20px;
  font-size: 15px;
  line-height: 24px;
  color: #737373;
}

.site-footer hr {
  border-top-color: #bbb;
  opacity: 0.5
}

.site-footer hr.small {
  margin: 20px 0
}

.site-footer h6 {
  color: #fff;
  font-size: 16px;
  text-transform: uppercase;
  margin-top: 5px;
  letter-spacing: 2px
}

.site-footer a {
  color: #737373;
}

.site-footer a:hover {
  color: #3366cc;
  text-decoration: none;
}

.footer-links {
  padding-left: 0;
  list-style: none
}

.footer-links li {
  display: block
}

.footer-links a {
  color: #737373
}

.footer-links a:active, .footer-links a:focus, .footer-links a:hover {
  color: #3366cc;
  text-decoration: none;
}

.footer-links.inline li {
  display: inline-block
}

.site-footer .social-icons {
  text-align: right
}

.site-footer .social-icons a {
  width: 40px;
  height: 40px;
  line-height: 40px;
  margin-left: 6px;
  margin-right: 0;
  border-radius: 100%;
  background-color: #33353d
}

.copyright-text {
  margin: 0
}



@media (max-width: 767px) {
  .site-footer {
    padding-bottom: 0
  }

  .site-footer .copyright-text, .site-footer .social-icons {
    text-align: center
  }
}

@media (max-width: 991px) {
  .site-footer [class^=col-] {
    margin-bottom: 30px
  }
}
.social-icons {
  padding-left: 0;
  margin-bottom: 0;
  list-style: none
}

.social-icons li {
  display: inline-block;
  margin-bottom: 4px
}

.social-icons li.title {
  margin-right: 15px;
  text-transform: uppercase;
  color: #96a2b2;
  font-weight: 700;
  font-size: 13px
}

.social-icons a {
  background-color: #eceeef;
  color: #818a91;
  font-size: 16px;
  display: inline-block;
  line-height: 44px;
  width: 44px;
  height: 44px;
  text-align: center;
  margin-right: 8px;
  border-radius: 100%;
  -webkit-transition: all .2s linear;
  -o-transition: all .2s linear;
  transition: all .2s linear
}

.social-icons a:active, .social-icons a:focus, .social-icons a:hover {
  color: #fff;
  background-color: #29aafe;

}

.social-icons.size-sm a {
  line-height: 34px;
  height: 34px;
  width: 34px;
  font-size: 14px
}

.social-icons a.github:hover {
  background-color: var(--clr-black)
}

.social-icons a.linkedin:hover {
  background-color: #007bb6
}

a.ubuntu {
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -ms-flex-line-pack: center;
  align-content: center;
  display: inline-block;
  color: darkorange;
  /*-webkit-transition: all .2s linear;*/
  /*-o-transition: all .2s linear;*/
  /*transition: all .2s linear;*/
  /*animation: ubuntu-rotation 5s infinite ease-out;*/
}

a.ubuntu:hover {
  -webkit-transition: var(--transition);
  -o-transition: var(--transition);
  transition: var(--transition);
  color: red;
}


@keyframes ubuntu-rotation {
  0% {
    /*transform: rotateY(0);*/
    color: orangered;
    -webkit-transform: scale(0.5);
    transform: scale(0.5);
  }
  50% {

    color: red;
    -webkit-transform: scale(1.1);
    transform: scale(1.1);


  }
  100% {
    /*transform: rotateY(180deg);*/
    color: orangered;
    -webkit-transform: scale(0.5);
    transform: scale(0.5);

  }
}

@-webkit-keyframes ubuntu-rotation {
  0% {
    -webkit-transform: rotateY(0);
    transform: rotateY(0);
    color: orangered;
  }
  50% {
    color: darkorange;
  }
  100% {
    -webkit-transform: rotateY(360deg);
    transform: rotateY(360deg);
    color: orangered;
  }
}

@media (max-width: 767px) {
  .social-icons li.title {
    display: block;
    margin-right: 0;
    font-weight: 600
  }
}

#footer {
  padding-top: 10px;
}

@media (max-width: 599px) {
  #footer {
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-pack: center;
    -ms-flex-pack: center;
    justify-content: center;
    -ms-flex-line-pack: center;
    align-content: center;
    font-size: 12px;
  }
}

</style>