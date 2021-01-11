<template>
  <div>
    <PastMainPicture></PastMainPicture>
    <PastAboutMe></PastAboutMe>
    <PastCarousel></PastCarousel>
    <MdbCarousel></MdbCarousel>
  </div>
</template>
<script>
import PastMainPicture from "@/components/PastMainPicture";
import PastAboutMe from "@/components/PastAboutMe";
import PastCarousel from "@/components/PastCarousel";
import MdbCarousel from "@/components/MdbCarousel";

export default {
  components: {
    PastMainPicture,
    PastAboutMe,
    PastCarousel,
    MdbCarousel
  }
}
</script>
<style scoped>

</style>