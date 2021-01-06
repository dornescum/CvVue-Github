<template>
  <div>
  <PastMainPicture></PastMainPicture>
    <PastAboutMe></PastAboutMe>
    <PastCarousel></PastCarousel>
  </div>
</template>
<script>
import PastMainPicture from "@/components/PastMainPicture";
import PastAboutMe from "@/components/PastAboutMe";
import PastCarousel from "@/components/PastCarousel";
export default {
  components:{
    PastMainPicture,
    PastAboutMe,
    PastCarousel
  }
}
</script>
<style scoped>

</style>