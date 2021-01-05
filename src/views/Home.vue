<template>
  <div class="home">

    <MainPicture />
    <HomeSkills></HomeSkills>
    <HomeAboutMe></HomeAboutMe>
  </div>
</template>

<script>
// @ is an alias to /src
import MainPicture from '@/components/MainPicture.vue'
import HomeSkills from "@/components/HomeSkills";
import HomeAboutMe from "@/components/HomeAboutMe";

export default {
  name: 'Home',
  components: {
    MainPicture,
    HomeSkills,
    HomeAboutMe
  }
}
</script>
