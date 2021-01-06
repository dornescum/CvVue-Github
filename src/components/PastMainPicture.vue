<template>
  <section class="hero" id="past">
    <div class="hero-container" id="past-container">

      <h6>
        “The past explains how I got here,
        but the future is up to me – and I love to
        live life at full throttle.”</h6>

    </div>
  </section>
</template>

<script>
export default {
  name: "PastMainPicture"
}
</script>

<style scoped>
#past {
  min-height: 50vh;
  /*margin-top: -6rem;*/
  background: -webkit-gradient(linear, left top, left bottom, from(rgba(0, 0, 0, 0.5)), to(rgba(0, 0, 0, 0.1))), url('../assets/webp/sg-min-min.webp') center/cover;
  background: -o-linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.1)), url('../assets/webp/sg-min-min.webp') center/cover;
  /*background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.1)), url('../assets/webp/sg-min-min.webp') center/cover;*/
  background:linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.1)),url('../assets/webp/sg-min-min.webp') left 30% bottom 35%/cover no-repeat border-box;

}

</style>