<template>
  <button class="Button" :disabled="loading">

  </button>
</template>

<script>
export default {
  name: "Loader",
  props: {
    loading: { type: Boolean }
  },
  data() {
    return {
      // loading: 'true'
    }
  },
  methods: {
    stopLoading() {

      setTimeout(() => {
        this.loading.classList.add('hide-loading')
      }, 1000)
    }

  }
}
</script>

<style scoped>
.loading {
  min-height: 20vh;
  min-width: 20vw;
  display: grid;
  justify-content: center;
  position: absolute;
  object-fit: fill;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: var(--clr-grey-10);
  padding-top: 5rem;
  z-index: 999;
}

.hide-loading {
  display: none;
}

</style>