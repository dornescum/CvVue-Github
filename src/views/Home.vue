<template>
  <div class="home">
    <MainPicture />
    <HomeSkills></HomeSkills>
    <HomeAboutMe></HomeAboutMe>
    <HomeProjects></HomeProjects>
  </div>
</template>

<script>
// @ is an alias to /src
import MainPicture from '@/components/MainPicture.vue'
import HomeSkills from "@/components/HomeSkills";
import HomeAboutMe from "@/components/HomeAboutMe";
import HomeProjects from "@/components/HomeProjects";

export default {
  name: 'Home',
  components: {
    MainPicture,
    HomeSkills,
    HomeAboutMe,
    HomeProjects
  }
}
</script>
