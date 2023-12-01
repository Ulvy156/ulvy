<template>
    <div id="aboutme" class="grid grid-cols-1">
        <h1 class="text-[50px] gradient underline md:text-[40px] sm:text-[30px] lg:text-[50px] xl:text-[50px] font-[600]">About Me</h1>
        <p class="text-[18px]">Hello there! 👋 I'm Ulvy, a passionate web developer with a love for crafting clean and functional websites. My journey in the world of web development began with a fascination for turning ideas into reality through code.</p>
        <ExperiencesCom/>
        <EducationCom/>
    </div>
</template>

<script>
import ExperiencesCom from './ExperiencesCom.vue';
import EducationCom from './EducationCom.vue';
export default {
    components:{
        ExperiencesCom,
        EducationCom
    }
}
</script>