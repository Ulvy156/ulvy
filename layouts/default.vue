<!-- layouts/default.vue -->
<template>
<div class="dark:bg-black">
    <!-- Your header content -->
    <header class="w-full fixed top-0 z-[990]">
        <NavBar />
    </header>

    <!-- main content -->
    <main class="min-h-screen w-full sm:mt-[78px] md:mt-[70px] lg:mt-[70px] xl:mt-[80px] mb-10 dark:text-white dark:bg-black">
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
