<template>
  <div class="home">
    <MainPicture />
    <HomeSkills></HomeSkills>
    <HomeAboutMe></HomeAboutMe>
<!--    <HomeProjects></HomeProjects>-->
    <HomeVFor></HomeVFor>
  </div>
</template>

<script>
// @ is an alias to /src
import MainPicture from '@/components/MainPicture.vue'
import HomeSkills from "@/components/HomeSkills";
import HomeAboutMe from "@/components/HomeAboutMe";
// import HomeProjects from "@/components/HomeProjects";
import HomeVFor from "@/components/HomeVFor";

export default {
  name: 'Home',
  components: {
    MainPicture,
    HomeSkills,
    HomeAboutMe,
    // HomeProjects,
    HomeVFor
  }
}
</script>
