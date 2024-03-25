<template>
    <Navbar/>
    <SubmitApplication/>
    <OurServices/>
    <OurWorks/>
    <Contacts/>
    <Footer/>
</template>

<script>

import Navbar from "@/components/Navbar.vue";
import SubmitApplication from "@/components/SubmitApplication.vue";
import OurServices from "@/components/OurServices.vue";
import OurWorks from "@/components/OurWorks.vue";
import Contacts from "@/components/Contacts.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: 'App',
    components: {Footer, Contacts, OurWorks, OurServices, SubmitApplication, Navbar},
}
</script>

<style>
#app {
    font-family: "Montserrat";
    background: linear-gradient(#333333, #1A1A1A);
}
</style>
