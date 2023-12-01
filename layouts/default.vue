<!-- layouts/default.vue -->
<template>
<div>
    <!-- Your header content -->
    <header class="w-full fixed top-0 z-[990]">
        <NavBar />
    </header>

    <!-- main content -->
    <main class="min-h-screen w-full sm:mt-[78px] md:mt-[70px] lg:mt-[68px] xl:mt-[70px] mb-10">
        <Nuxt />
    </main>

    <!-- footer content -->
    <footer class="w-full">
        <FooterCom />
    </footer>
</div>
</template>

<script>
import NavBar from "~/components/NavBar.vue"
import FooterCom from "~/components/FooterCom.vue"
export default {
    components: {
        NavBar,
        FooterCom
    },
 
}
</script>

<style>
/* english font */
@import url('https://fonts.cdnfonts.com/css/gill-sans-mt-2');
/* ============= */

body {
    font-family: 'Gill Sans MT', sans-serif;
    padding: 0;
    margin: 0;
}
</style>
