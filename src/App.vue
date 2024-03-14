<template>
<Navbar/>
<SubmitApplication/>
<OurServices/>
</template>

<script>

import Navbar from "@/components/Navbar.vue";
import SubmitApplication from "@/components/SubmitApplication.vue";
import OurServices from "@/components/OurServices.vue";

export default {
  name: 'App',
    components: {OurServices, SubmitApplication, Navbar},
}
</script>

<style>
#app {
    font-family: "Montserrat";
    background: linear-gradient(#333333, #1A1A1A);
}
</style>
