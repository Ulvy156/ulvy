<!-- Please remove this file from your project -->
<template>
<div class="grid grid-cols-1 gap-y-10">
    <ImageHome/>
    <AboutMe/>
    <SkillCom/>
    <ContactMe/>
</div>
</template>

<script>
import ImageHome from "~/components/ImageHome.vue"
import AboutMe from "~/components/AboutMe.vue";
import SkillCom from "~/components/SkillCom.vue"
import ContactMe from "~/components/ContactMe.vue";
export default {
  components:{
    ImageHome,
    AboutMe,
    SkillCom,
    ContactMe
  }
}
</script>


<style >
.gradient{
    background-image: linear-gradient(to right, #82B2FA 0%, #6393C1 100%);
    -webkit-background-clip: text; /* For Safari */
    -moz-background-clip: text; /* For Firefox */
    -webkit-text-fill-color: transparent; /* Fix for older Safari versions */
    color: transparent;
}
</style>
