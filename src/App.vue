<template>
<Navbar/>
<SubmitApplication/>
</template>

<script>

import Navbar from "@/components/Navbar.vue";
import SubmitApplication from "@/components/SubmitApplication.vue";

export default {
  name: 'App',
    components: {SubmitApplication, Navbar},
}
</script>

<style>
#app {
    font-family: "Montserrat";
}
</style>
