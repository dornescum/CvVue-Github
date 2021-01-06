<template>
  <div>
    <section id="container-repo" v-for="project in projects" :key="project.id">
      <div class="title">
        <!--    titlu-->
        <h2>Some Projects</h2>
        <div class="underline"></div>

        <!--    despre-->
        <article class="projects" >
          <div class="img-container">
            <img :src=project.img id="person-img" alt="">
          </div>
          <h4 id="author">{{ project.name}}</h4>
          <p id="source">{{project.source}}</p>
          <p id="info">{{project.text}}</p>
          <!--        prev next btn-->
          <div class="button-container">
            <button class="prev-btn">
              <i class="fas fa-chevron-left"></i>
            </button>
            <button class="next-btn" @click="moveRight">
              <i class="fas fa-chevron-right"></i>
            </button>
          </div>
        </article>
      </div>
    </section>
  </div>
</template>

<script>

export default {
name: "HomeProjects",
  components:{
  },
  data(){
  return{
    buttonRight: true,
    buttonLeft: true,
    count : 0,
    projects : [
      {
        id: 1,
        name: "Mihai Dornescu",
        source: "Udemy",
        img: 'https://images.unsplash.com/photo-1461749280684-dccba630e2f6?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1050&q=80',
        text: '            Lorem ipsum dolor sit ame' +
            't, consectetur adipisicing elit. Accusantium, adip' +
            'isci, assumenda deleniti deserunt dolore dolorum eos hic' +
            ' laudantium minima mollitia odit praesentium, quidem ' +
            'repellat repellendus saepe tempore ut vel velit.'
      },
      {
        id: 2,
        name: "Mihai Dornescu",
        source: "Youtube",
        img: 'https://images.unsplash.com/photo-1587620962725-abab7fe55159?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1189&q=80',
        text: '   “Lorem ipsum” dummy text is used by many web-developers to test ' +
            'how their HTML templates will look with real data. Often, developers use ' +
            'third-party services to generate “Lorem ipsum” text, but now you can do that ' +
            'right in your editor. Just expand lorem or lipsum abbreviations to get the following snippet:'
      },
      {
        id: 3,
        name: "Mihai Dornescu",
        source: "GitHub",
        img: 'https://images.unsplash.com/photo-1593720217529-01f0a5d09aed?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1008&q=80',
        text: '           Lorem ipsum dolor sit amet, consectetur adipisicing elit. ' +
            'Eligendi non quis exercitationem culpa nesciunt nihil aut nostrum explicabo' +
            ' reprehenderit optio amet ab temporibus asperiores quasi cupiditate. Voluptatum ' +
            'ducimus voluptates voluptas?'
      },
      {
        id: 4,
        name: "Mihai Dornescu",
        source: "Udemy",
        img: 'https://images.unsplash.com/photo-1593720213428-28a5b9e94613?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1050&q=80',
        text: '  Lorem Ipsum is simply dummy text of the printing and typesetting industry. ' +
            'Lorem Ipsum has been the industry\'s standard dummy text ever since the 1500s, ' +
            'when an unknown printer took a galley of type and scrambled it to make a type ' +
            'specimen book. It has survived not only five centuries, but also the leap into ' +
            'electronic typesetting, remaining essentially unchanged. It was popularised in the ' +
            '1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more '

      },
    ]
  }
  },
  methods:{
  moveRight(){

  }
  }
}
</script>

<style scoped>
#container-repo {
  width: 80vw;
  /*max-width: var(--fixed-width);*/
}

.projects {
  background: var(--clr-white);
  padding: 1.5rem 2rem;
  border-radius: var(--radius);
  -webkit-box-shadow: var(--light-shadow);
  box-shadow: var(--light-shadow);
  -webkit-transition: var(--transition);
  -o-transition: var(--transition);
  transition: var(--transition);
  text-align: center;
}

.projects:hover {
  -webkit-box-shadow: var(--dark-shadow);
  box-shadow: var(--dark-shadow);
}

.img-container {
  position: relative;
  width: 170px;
  height: 150px;
  border-radius: 50%;
  margin: 0 auto;
  margin-bottom: 1.5rem;
}

#person-img {
  width: 100%;
  display: block;
  height: 100%;
  -o-object-fit: cover;
  object-fit: cover;
  border-radius: 10%;
  position: relative;
}

.img-container::after {
  font-family: "Font Awesome 5 Free";
  font-weight: 900;
  content: "\f10e";
  position: absolute;
  top: 0;
  left: 0;
  width: 2.5rem;
  height: 2.5rem;
  display: -ms-grid;
  display: grid;
  place-items: center;
  border-radius: 10%;
  -webkit-transform: translateY(15%);
  -ms-transform: translateY(15%);
  transform: translateY(15%);
  background: var(--clr-primary-5);
  color: var(--clr-white);
}

.img-container::before {
  content: "";
  width: 100%;
  height: 100%;
  background: var(--clr-primary-5);
  position: absolute;
  top: -0.25rem;
  right: -0.35rem;
  border-radius: 10%;
}

#author {
  margin-bottom: 0.25rem;
}

#source {
  margin-bottom: 0.5rem;
  text-transform: uppercase;
  color: var(--clr-primary-5);
  font-size: 0.85rem;
}

#info {
  margin-bottom: 0.75rem;
}

.prev-btn,
.next-btn {
  color: var(--clr-primary-7);
  font-size: 1.25rem;
  background: transparent;
  border-color: transparent;
  margin: 0 0.5rem;
  -webkit-transition: var(--transition);
  -o-transition: var(--transition);
  transition: var(--transition);
  cursor: pointer;
}

.prev-btn:hover,
.next-btn:hover {
  color: var(--clr-primary-5);
}

</style>