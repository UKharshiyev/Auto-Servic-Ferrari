<template>
    <Navbar/>
    <SubmitApplication/>
    <OurServices/>
    <OurWorks/>
</template>

<script>

import Navbar from "@/components/Navbar.vue";
import SubmitApplication from "@/components/SubmitApplication.vue";
import OurServices from "@/components/OurServices.vue";
import OurWorks from "@/components/OurWorks.vue";

export default {
  name: 'App',
    components: {OurWorks, OurServices, SubmitApplication, Navbar},
}
</script>

<style>
#app {
    font-family: "Montserrat";
    background: linear-gradient(#333333, #1A1A1A);
}
</style>
