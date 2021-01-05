<template>
  <div class="container" id="progress">
    <h6 class="text-center mt-3">Skills</h6>
    <div class="row ">
      <div class="col-lg-6">
        <div class="container">
          <p>Html</p>
          <div class="skills">
            <span class="value" id="html">80%</span>
          </div>
          <p>Css</p>
          <div class="skills">
            <span class="value" id="css">70%</span>
          </div>
          <p>Vanill Js </p>
          <div class="skills">
            <span class="value" id="js">50%</span>
          </div>

        </div>
      </div>
      <div class="col-lg-6 ">
        <div class="container">
          <p>React js</p>
          <div class="skills">
            <span class="value" id="react">20%</span>
          </div>
          <p>TypeScript</p>
          <div class="skills">
            <span class="value" id="typeScript">5%</span>
          </div>
          <p>Vue js</p>
          <div class="skills">
            <span class="value" id="vuejs">45%</span>
          </div>

        </div>
      </div>

      <div class="col-lg-6">
        <div class="container">
          <p>Sass</p>
          <div class="skills">
            <span class="value" id="sass">40%</span>
          </div>
        </div>
      </div>
      <div class="col-lg-6 ">
        <div class="container">
          <p>Pwa</p>
          <div class="skills">
            <span class="value" id="pwa">10%</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Skills"
}
</script>

<style scoped>
#progress {
  /*background: rgb(74,71,122);*/
  /*background: linear-gradient(90deg, rgba(192, 182, 207, 0.3723506284563729) 0%, rgba(233, 205, 205, 0.6476315273327774) 9%, rgba(226, 226, 244, 0.7459461340743504) 19%, rgba(166, 193, 202, 0.6448225385687325) 35%, rgba(165, 212, 212, 0.9369573700294066) 48%, rgba(174, 190, 193, 0.7010023138496313) 68%, rgba(224, 231, 232, 0.816170853175474) 84%, rgba(198, 210, 212, 0.765609055422665) 92%, rgba(209, 230, 234, 0.8948225385687325) 97%, rgba(198, 222, 227, 1) 100%);*/
  /*background: linear-gradient(90deg, rgba(102,101,104,0.3723506284563729) 0%, rgba(27,27,28,0.6476315273327774) 9%, rgba(27,27,42,0.7459461340743504) 19%, rgba(57,73,78,0.6448225385687325) 35%, rgba(24,37,37,0.8302456724877451) 48%, rgba(20,21,21,0.7010023138496313) 68%, rgba(34,45,46,0.816170853175474) 84%, rgba(27,30,31,0.765609055422665) 92%, rgba(43,45,48,0.8948225385687325) 97%, rgba(76,76,78,1) 100%);*/
  background: -webkit-gradient(linear, left top, right top, from(var(--clr-grey-9)), to(var(--clr-grey-10)));
  background: -o-linear-gradient(left, var(--clr-grey-9), var(--clr-grey-10));
  background: linear-gradient(to right, var(--clr-grey-9), var(--clr-grey-10));
  -webkit-box-shadow: var(--light-shadow);
  box-shadow: var(--light-shadow);
  -webkit-transition: var(--transition);
  -o-transition: var(--transition);
  transition: var(--transition);
  border-radius: var(--radius);
  max-width: 80vw;
}

#progress:hover {
  -webkit-box-shadow: var(--dark-shadow);
  box-shadow: var(--dark-shadow);
}

/*progress bar*/
span {
  /*background-color: orangered;*/
  height: 30px;
  display: block;
  -webkit-animation: progressBar 2s linear forwards;
  animation: progressBar 2s linear forwards;
  border-radius: 15px;
  text-align: start;
  padding-left: 20px;
  margin: 10px;
}

#html {
  background-color: orangered;
  -webkit-animation: progressBar 2s linear forwards;
  animation: progressBar 2s linear forwards;
}

#css {
  background-color: #2862E9;
  -webkit-animation: progressBarCss 2s linear forwards;
  animation: progressBarCss 2s linear forwards;
}

#js {
  background-color: #F7E017;
  -webkit-animation: progressBarJs 2s linear forwards;
  animation: progressBarJs 2s linear forwards;
}

#react {
  background-color: #61DBFB;
  -webkit-animation: progressBarReact 2s linear forwards;
  animation: progressBarReact 2s linear forwards;
}

#typeScript {
  background-color: #61DBFB;
  -webkit-animation: progressBarTypeScript 5s linear forwards;
  animation: progressBarTypeScript 5s linear forwards;
}

#vuejs {
  background-color: #0576C5;
  -webkit-animation: progressBarVue 5s linear forwards;
  animation: progressBarVue 5s linear forwards;
}
#sass {
  background-color: #CF649A;
  -webkit-animation: progressBarSass 5s linear forwards;
  animation: progressBarSass 5s linear forwards;
}
#pwa {
  background-color: #ccc;
  -webkit-animation: progressBarPwa 5s linear forwards;
  animation: progressBarPwa 5s linear forwards;
}

@keyframes progressBar {
  0% {
    width: 0;
    /*box-shadow: 0 0 30px blue;*/
  }
  100% {
    width: 80%;
    /*box-shadow: 0 0 30px green;*/
  }
}

@-webkit-keyframes progressBar {
  0% {
    width: 0;
    /*box-shadow: 0 0 30px blue;*/
  }
  100% {
    width: 80%;
    /*box-shadow: 0 0 30px green;*/
  }
}

@keyframes progressBarCss {
  0% {
    width: 0;
    -webkit-box-shadow: 0 0 30px blue;
    box-shadow: 0 0 30px blue;
  }
  100% {
    width: 70%;
    -webkit-box-shadow: 0 0 30px green;
    box-shadow: 0 0 30px green;
  }
}

@-webkit-keyframes progressBarCss {
  0% {
    width: 0;
    -webkit-box-shadow: 0 0 30px blue;
    box-shadow: 0 0 30px blue;
  }
  100% {
    width: 70%;
    -webkit-box-shadow: 0 0 30px green;
    box-shadow: 0 0 30px green;
  }
}

@keyframes progressBarJs {
  0% {
    width: 0;
    -webkit-box-shadow: 0 0 30px blue;
    box-shadow: 0 0 30px blue;
  }
  100% {
    width: 50%;
    -webkit-box-shadow: 0 0 30px green;
    box-shadow: 0 0 30px green;
  }
}

@-webkit-keyframes progressBarJs {
  0% {
    width: 0;
    -webkit-box-shadow: 0 0 30px blue;
    box-shadow: 0 0 30px blue;
  }
  100% {
    width: 50%;
    -webkit-box-shadow: 0 0 30px green;
    box-shadow: 0 0 30px green;
  }
}

@keyframes progressBarReact {
  0% {
    width: 0;
    -webkit-box-shadow: 0 0 30px blue;
    box-shadow: 0 0 30px blue;
  }
  100% {
    width: 30%;
    -webkit-box-shadow: 0 0 30px green;
    box-shadow: 0 0 30px green;
  }
}

@-webkit-keyframes progressBarReact {
  0% {
    width: 0;
    -webkit-box-shadow: 0 0 30px blue;
    box-shadow: 0 0 30px blue;
  }
  100% {
    width: 30%;
    -webkit-box-shadow: 0 0 30px green;
    box-shadow: 0 0 30px green;
  }
}

@keyframes progressBarReactNative {
  0% {
    width: 0;
    -webkit-box-shadow: 0 0 30px blue;
    box-shadow: 0 0 30px blue;
  }
  50% {
    width: 100%;
    -webkit-box-shadow: 0 0 30px green;
    box-shadow: 0 0 30px green;
  }
  100% {
    width: 5%;
    -webkit-box-shadow: 0 0 30px blue;
    box-shadow: 0 0 30px blue;
  }
}

@-webkit-keyframes progressBarReactNative {
  0% {
    width: 0;
    -webkit-box-shadow: 0 0 30px blue;
    box-shadow: 0 0 30px blue;
  }
  50% {
    width: 100%;
    -webkit-box-shadow: 0 0 30px green;
    box-shadow: 0 0 30px green;
  }
  100% {
    width: 5%;
    -webkit-box-shadow: 0 0 30px blue;
    box-shadow: 0 0 30px blue;
  }
}

@keyframes progressBarTypeScript {
  0% {
    width: 0;
    -webkit-box-shadow: 0 0 30px blue;
    box-shadow: 0 0 30px blue;
  }
  50% {
    width: 100%;
    -webkit-box-shadow: 0 0 30px green;
    box-shadow: 0 0 30px green;
  }
  100% {
    width: 5%;
    -webkit-box-shadow: 0 0 30px blue;
    box-shadow: 0 0 30px blue;
  }
}

@-webkit-keyframes progressBarTypeScript {
  0% {
    width: 0;
    -webkit-box-shadow: 0 0 30px blue;
    box-shadow: 0 0 30px blue;
  }
  50% {
    width: 100%;
    -webkit-box-shadow: 0 0 30px green;
    box-shadow: 0 0 30px green;
  }
  100% {
    width: 5%;
    -webkit-box-shadow: 0 0 30px blue;
    box-shadow: 0 0 30px blue;
  }
}

@keyframes progressBarVue {
  0% {
    width: 0;
    -webkit-box-shadow: 0 0 30px blue;
    box-shadow: 0 0 30px blue;
  }
  50% {
    width: 100%;
    -webkit-box-shadow: 0 0 30px green;
    box-shadow: 0 0 30px green;
  }
  100% {
    width: 45%;
    -webkit-box-shadow: 0 0 30px blue;
    box-shadow: 0 0 30px blue;
  }
}

@-webkit-keyframes progressBarVue {
  0% {
    width: 0;
    -webkit-box-shadow: 0 0 30px blue;
    box-shadow: 0 0 30px blue;
  }
  50% {
    width: 100%;
    -webkit-box-shadow: 0 0 30px green;
    box-shadow: 0 0 30px green;
  }
  100% {
    width: 45%;
    -webkit-box-shadow: 0 0 30px blue;
    box-shadow: 0 0 30px blue;
  }
}

@keyframes progressBarSass {
  0% {
    width: 0;
    -webkit-box-shadow: 0 0 30px blue;
    box-shadow: 0 0 30px blue;
  }
  50% {
    width: 100%;
    -webkit-box-shadow: 0 0 30px blue;
    box-shadow: 0 0 30px blue;
  }
  100% {
    width: 35%;
    -webkit-box-shadow: 0 0 30px blue;
    box-shadow: 0 0 30px blue;
  }
}

@-webkit-keyframes progressBarSass {
  0% {
    width: 0;
    -webkit-box-shadow: 0 0 30px blue;
    box-shadow: 0 0 30px blue;
  }
  50% {
    width: 100%;
    -webkit-box-shadow: 0 0 30px green;
    box-shadow: 0 0 30px green;
  }
  100% {
    width: 35%;
    -webkit-box-shadow: 0 0 30px blue;
    box-shadow: 0 0 30px blue;
  }
}

@keyframes progressBarPwa {
  0% {
    width: 0;
    -webkit-box-shadow: 0 0 30px blue;
    box-shadow: 0 0 30px blue;
  }
  50% {
    width: 100%;
    -webkit-box-shadow: 0 0 30px green;
    box-shadow: 0 0 30px green;
  }
  100% {
    width: 10%;
    -webkit-box-shadow: 0 0 30px blue;
    box-shadow: 0 0 30px blue;
  }
}

@-webkit-keyframes progressBarPwa {
  0% {
    width: 0;
    -webkit-box-shadow: 0 0 30px blue;
    box-shadow: 0 0 30px blue;
  }
  50% {
    width: 100%;
    -webkit-box-shadow: 0 0 30px green;
    box-shadow: 0 0 30px green;
  }
  100% {
    width: 10%;
    -webkit-box-shadow: 0 0 30px blue;
    box-shadow: 0 0 30px blue;
  }
}



.skills {
  position: relative;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  margin: 20px 0;
  padding:  10px 10px;
  background: -webkit-gradient(linear, left top, left bottom, from(#626262), color-stop(10%, #333), to(#222));
  background: -o-linear-gradient(#626262 0%, #333 10%, #222);
  background: linear-gradient(#626262 0%, #333 10%, #222);
  border-radius: 8px;
  overflow: hidden;
  border: black 2px solid;
  -webkit-transition: var(--transition);
  -o-transition: var(--transition);
  transition: var(--transition);
}

.skills .value {
  position: relative;
  width: 40px;
  text-align: left;
  color: var(--clr-white);
  /*margin-top: -2px;*/
}


</style>