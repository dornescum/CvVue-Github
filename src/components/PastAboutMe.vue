<template>

  <!--despre mine imagine-->
  <section id="past-aboutMe">
    <div class="container mt-3 mb-5">
      <!--    despre mine-->
      <h3 class="mt-1">About me</h3>
      <p class="text-aboutMe">
        After 20 years of experience, in the kitchens of restaurants in Romania and France, I returned home and was preparing to have my own business, but the pandemic came...
        Being an active person, passionate about the IT field and with a creative spirit, I decided that it is an opportune moment to start on another path and build a career in the IT field that I am passionate about, realizing that it will not be easy.
        I am an old Linux user and for the beginning I turned my attention to front end development.
        For personal development I adopted the self teaching method with Github, Udemy, Mdn web docs and Youtube as information resources.
        I started with Html and Css courses and exercises and continued with Bootstrap and  MaterializeCss.
        After a few months of intense study, practice and practice, the next steps were towards Javascript and I discovered dynamic content and I that I like the idea of manipulating the content with the help of the browser.
        At the moment I am perfecting my knowledge with the Vue js framework… and the next steps will be   Typescript and React js.
        My goal is to find a job in this field where I can learn new things.


      </p>
      <!--    slider-->
      <div class="row mb-3">
        <div class="col-lg-4 col-md-4 col-sm-12 ">
          <img src="../assets/webp/unemployed.png" alt="unemployed" id="unemployed" >
        </div>
        <div class="col-lg-4 col-md-4 col-sm-12 ">
          <img src="../assets/webp/jobless.webp" alt="" id="jobless">
        </div>
        <div class="col-lg-4 col-md-4 col-sm-12 ">
          <img src="../assets/webp/study.webp" alt="" id="study">
        </div>

      </div>
    </div>
  </section>

</template>

<script>
export default {
name: "PastAboutMe"
}
</script>

<style scoped>
/*todo nefixat width*/
#past-aboutMe{
  max-width: 100vw;
}
#unemployed {
  -webkit-filter: blur(2px);
  filter: blur(2px);
  -webkit-transition: var(--transition);
  -o-transition: var(--transition);
  transition: var(--transition);
  padding: 2px;
}

#unemployed:hover {
  -webkit-filter: blur(0px);
  filter: blur(0px);
  -webkit-transition: var(--transition);
  -o-transition: var(--transition);
  transition: var(--transition);
}

#jobless {
  -webkit-transform: scale(1);
  -ms-transform: scale(1);
  transform: scale(1);
  -webkit-transition: var(--transition);
  -o-transition: var(--transition);
  transition: var(--transition);
  padding: 2px;
}

#jobless:hover {
  -webkit-transform: scale(1.1);
  -ms-transform: scale(1.1);
  transform: scale(1.1);
  -webkit-transition: var(--transition);
  -o-transition: var(--transition);
  transition: var(--transition);
  padding: 2px;
}

#study {
  -webkit-transform: rotateY(0);
  transform: rotateY(0);
}

#study:hover {
  -webkit-transform: rotateY(180deg);
  transform: rotateY(180deg);
  -webkit-transition: var(--transition);
  -o-transition: var(--transition);
  transition: var(--transition);
}
img {
  width: 100%;
  /*height: 100%;*/
  -o-object-fit: cover;
  object-fit: cover;
  border-radius: var(--radius);
  cursor: pointer;
  -webkit-transition: var(--transition);
  -o-transition: var(--transition);
  transition: var(--transition);
  -webkit-box-shadow: var(--light-shadow);
  box-shadow: var(--light-shadow);
  height: 15rem;
}

</style>