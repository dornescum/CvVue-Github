<template>
  <section class="hero">
    <div class="hero-container">
      <a href="#" class="hero-btn" data-toggle="modal" data-target="#exampleModal">
        Learning
      </a>
      <!-- Modal -->
      <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
        <div class="modal-dialog">
          <div class="modal-content">
            <div class="modal-header">
              <h5 class="modal-title" id="exampleModalLabel">Certificari</h5>
              <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                <span aria-hidden="true">&times;</span>
              </button>
            </div>
            <div class="modal-body">
              <h1>html</h1>
              <img src="img/webp/udemyHmtlCss%20(1).webp" alt="html">
              <img src="img/webp/css.webp" alt="css">
              <img src="img/js.png" alt="js">
              <img src="img/webp/bootstrap.webp" alt="bootstrap">
              <img src="img/webp/materializeCss.webp" alt="materializeCss">


            </div>
            <div class="modal-footer">
              <button type="button" class="btn btn-secondary" data-dismiss="modal">Close</button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {

    };
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hero {
  min-height: 100vh;
  margin-top: -6rem;
  background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.1)), url('../assets/webp/Learning.webp') center/cover;
  display: grid;
  place-items: center;
  color: var(--clr-white);
}

.hero-container {
  width: 80vw;
  max-width: var(--max-width);
}

.hero h1 {
  font-weight: 700;
}

.hero h3 {
  text-transform: none;
  font-size: 1.5rem;
}

.hero-btn {
  color: var(--clr-white);
  background: transparent;
  border: 1px solid var(--clr-white);
  padding: 0.1rem 0.75rem;
  display: inline-block;
  /*margin-top: 0.75rem;*/
  text-transform: uppercase;
  letter-spacing: var(--spacing);
  border-radius: var(--radius);
  transition: var(--transition);
}

.hero-btn:hover {
  background: var(--clr-white);
  color: var(--clr-primary-5);
}

</style>
