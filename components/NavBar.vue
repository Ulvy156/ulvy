<template>
<div class="md:grid sm:grid xl:grid lg:grid lg:grid-cols-3 xl:grid-cols-3 sm:grid-cols-1 md:grid-cols-2 py-3 sm:px-1 md:px-1 lg:px-7 xl:px-7 border-b-1 border border-gray-600 border-x-0 border-t-0 bg-white">

    <div class="flex justify-between items-center text-lg lg:w-1/43  xl:w-1/4 sm:w-full md:w-1/2 " >
        <div class="flex justify-between items-center cursor-pointer" @click="scrollToSection('homepage')">
            <span class="pi pi-home"></span>
            <button class="ml-2 mt-[3px]" >Home</button>
        </div>
        <div class="flex justify-between items-center cursor-pointer" @click="scrollToSection('aboutme')">
            <span class="pi pi-user"></span>
            <button class="ml-2 mt-1" >About</button>
        </div>
        <div class="flex justify-between items-center cursor-pointer" @click="scrollToSection('skills')">
            <span class="pi pi-code"></span>
            <button class="ml-2" >Skills</button>
        </div>
        <div class="flex justify-between items-center cursor-pointer" @click="scrollToSection('contact')">
            <span class="pi pi-phone"></span>
            <button class="ml-2" >Contact</button>
        </div>
    </div>

    <div class="w-1/2"></div>
</div>

</template>

<script>
import {
    scrollTo
} from 'vue-scrollto';

export default {

    data() {
        return {
            items: [{
                    label: 'Home',
                    icon: 'pi pi-home',
                    id:'homepage'
                },
                {
                    label: 'About Me',
                    icon: 'pi pi-user',
                    id:'aboutme'
                },
                {
                    label: 'Skills',
                    icon: 'pi pi-code',
                    id:'skills'
                }
            ]
        }
    },
    methods: {
        scrollToSection(sectionId) {
            scrollTo(`#${sectionId}`, 1000, {
                offset: -50, // Adjust the offset if needed
                easing: 'easeInOutCubic', // Easing function (optional)
            });
        },
    },
};
</script>
