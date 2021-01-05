<template>
  <div class="container" id="container">
    <div class="row m-2">
      <div class="col-lg-6 col-md-8">
        <div>
          <img src="../assets/webp/IMG_20191124_103021.webp" alt="temporar" id="poza">
        </div>
      </div>
      <div class="col-lg-6 col-md-4">
        <div>
          <p class="text fade1">
            Be willing to be a beginner every single morning.
            <br>
            <br>
            <a href="https://en.wikipedia.org/wiki/Meister_Eckhart" id="quote">
              Meister Eckhart
            </a>
            <br>
            <a href="./future.html">
              <button class="btn-main">
                JavaScript
              </button>
            </a>

          </p>

        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
name: "HomeAboutMe"
}
</script>

<style scoped>
/* culoare container despre mine  */

#container {
  background-color: var(--clr-grey-10);
  border-radius: var(--radius);
  -webkit-box-shadow: var(--light-shadow);
  box-shadow: var(--light-shadow);
  max-width: 80vw;
}

#container:hover {
  -webkit-box-shadow: var(--dark-shadow);
  box-shadow: var(--dark-shadow);
  -webkit-transition: var(--transition);
  -o-transition: var(--transition);
  transition: var(--transition);
}

#quote {
  color: black;
  padding-left: 150px
}
@media (min-width:768px){
  #quote {
    padding: 100px;
  }
}
@media (min-width:768px){
  #quote {
    padding: 50px;
  }
}

/* poza mea nu merge */
#poza {
  position: relative;
  -webkit-animation: poza 10s;
  animation: poza 10s;
  -webkit-animation-poza: 10s;
  -webkit-animation-fill-mode: forwards;
  animation-fill-mode: forwards;
  -webkit-transition: poza linear;
  -o-transition: poza linear;
  transition: poza linear;
  -webkit-filter: grayscale(100%);
  filter: grayscale(100%);

}

#poza:hover {
  -webkit-filter: grayscale(0);
  filter: grayscale(0);
  -webkit-transition: var(--transition);
  -o-transition: var(--transition);
  transition: var(--transition);

}

@keyframes poza {
  from {
    opacity: 0;
    -webkit-transform: translateY(100px);
    transform: translateY(100px);
  }
  to {
    opacity: 1;
    -webkit-transform: translateY(0px) scale(0.9);
    transform: translateY(0px) scale(0.9);
  }
}

@-webkit-keyframes poza {
  from {
    opacity: 0;
    -webkit-transform: translateY(100px);
    transform: translateY(100px);
  }
  to {
    opacity: 1;
    -webkit-transform: translateY(0px) scale(0.9);
    transform: translateY(0px) scale(0.9);
  }
}

.btn-main {
  color: var(--clr-white);
  background: var(--clr-primary-5);
  display: block;
  width: 90%;
  border-color: transparent;
  margin: 2rem auto 0 auto;
  text-transform: capitalize;
  font-size: 1.2rem;
  letter-spacing: var(--spacing);
  border-radius: var(--radius);
  -webkit-transition: var(--transition);
  -o-transition: var(--transition);
  transition: var(--transition);
  cursor: pointer;
  -webkit-box-shadow: var(--light-shadow);
  box-shadow: var(--light-shadow);
}

.btn-main:hover {
  background-color: var(--clr-primary-10);
  color: var(--clr-primary-5);
  -webkit-box-shadow: var(--dark-shadow);
  box-shadow: var(--dark-shadow);
  /*font-size: 1.3rem;*/
  border: none;
}
.fade1 {
  position: relative;
  -webkit-animation: top 3s;
  animation: top 3s;
  -webkit-animation-fill-mode: forwards;
  animation-fill-mode: forwards;
}
.text {
  color: var(--clr-black);
  font-size: 24px;
  letter-spacing: var(--spacing);
  position: absolute;
  top: 50%;
  left: 50%;
  -webkit-transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  text-align: center;
}
@media (max-width: 992px) {
  .fade1 {
    -webkit-animation: top 3s;
    animation: top 3s;
    -webkit-animation-fill-mode: forwards;
    animation-fill-mode: forwards;
  }

  .text {
    font-size: 16px;
  }

  @keyframes top {
    from {
      top: 0;
      opacity: 0;
      /*transform: translateY(100px);*/
    }
    to {
      top: 250px;
      opacity: 1;
      /*transform: translateY(-100px);*/
    }
  }
  @-webkit-keyframes top {
    from {
      top: 0;
      opacity: 0;
      /*transform: translateY(100px);*/
    }
    to {
      top: 250px;
      opacity: 1;
      /*transform: translateY(-100px);*/
    }
  }
}

@media screen and (max-width: 768px) {
  .fade1 {
    -webkit-animation: top 3s;
    animation: top 3s;
    -webkit-animation-fill-mode: forwards;
    animation-fill-mode: forwards;
  }

  .text {
    font-size: 14px;
  }


  @keyframes top {
    from {
      top: 0;
      opacity: 0;
      /*transform: translateY(100px);*/
    }
    to {
      top: 220px;
      opacity: 1;
      /*transform: translateY(-100px);*/
    }
  }
  @-webkit-keyframes top {
    from {
      top: 0;
      opacity: 0;
      /*transform: translateY(100px);*/
    }
    to {
      top: 220px;
      opacity: 1;
      /*transform: translateY(-100px);*/
    }
  }
}


@media (max-width: 599px) {
  .fade1 {
    -webkit-animation: top 3s;
    animation: top 3s;
    -webkit-animation-fill-mode: forwards;
    animation-fill-mode: forwards;
  }

  .text {
    font-size: 12px;
  }

  @keyframes top {
    from {
      top: 0;
      opacity: 0;
      /*transform: translateY(100px);*/
    }
    to {
      top: 100px;
      opacity: 1;
      /*transform: translateY(-100px);*/
    }
  }
  @-webkit-keyframes top {
    from {
      top: 0;
      opacity: 0;
      /*transform: translateY(100px);*/
    }
    to {
      top: 100px;
      opacity: 1;
      /*transform: translateY(-100px);*/
    }
  }}


</style>