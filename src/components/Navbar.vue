<template>
    <header>
        <nav class="navbar navbar-expand-lg">
            <div class="container-fluid ps-2 pe-0">
                <router-link class="navbar-brand text-light" to="/">
                    <img src="../assets/img/Logo.png" alt="LOGO"/>
                </router-link>
                <button
                        @click="isCloseNavbar = !isCloseNavbar"
                        class="navbar-toggler border-0"
                        type="button"
                        data-bs-toggle="collapse"
                        data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent"
                        aria-expanded="false" aria-label="Toggle navigation">
                        <svg v-if="!isCloseNavbar" xmlns="http://www.w3.org/2000/svg" width="40" height="40" fill="currentColor" class="bi bi-list" viewBox="0 0 16 16">
                            <path fill-rule="evenodd" d="M2.5 12a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5m0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5m0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5"/>
                        </svg>
                        <svg v-if="isCloseNavbar" xmlns="http://www.w3.org/2000/svg" width="40" height="40" fill="currentColor" class="bi bi-x-lg" viewBox="0 0 16 16">
                            <path d="M2.146 2.854a.5.5 0 1 1 .708-.708L8 7.293l5.146-5.147a.5.5 0 0 1 .708.708L8.707 8l5.147 5.146a.5.5 0 0 1-.708.708L8 8.707l-5.146 5.147a.5.5 0 0 1-.708-.708L7.293 8z"/>
                        </svg>
                </button>
                <div class="collapse navbar-collapse" id="navbarSupportedContent">
                    <ul class="navbar-nav text-center">
                        <li class="nav-item ps-lg-5 ms-lg-2 ms-xl-5">
                            <a class="nav-link text-white" href="#our-service">
                                Услуги
                            </a>
                        </li>
                        <li class="nav-item">
                            <router-link class="nav-link text-white" to="#">
                                Преимущества
                            </router-link>
                        </li>
                        <li class="nav-item">
                            <router-link class="nav-link text-white" to="#">
                                Наши работы
                            </router-link>
                        </li>
                        <li class="nav-item">
                            <router-link class="nav-link text-white" to="#">
                                Контакты
                            </router-link>
                        </li>
                    </ul>
                    <div class="ms-auto text-center">
                        <a class="nav-link text-white nav-item-end d-inline" href="tel:+79610438408">
                            +7 (961) 043-84-08
                        </a>
                        <a href="#" class="mx-2">
                            <img src="../assets/icons/whatsapp-icon.png" width="30" height="30">
                        </a>
                        <a href="#">
                            <img src="../assets/icons/telegram-icon.png" width="30" height="30" class="telegram-icon">
                        </a>
                    </div>

                </div>
            </div>
        </nav>
    </header>
</template>

<script>
export default {
    // eslint-disable-next-line
    name: "Navbar",
    data() {
        return {
            isCloseNavbar: false
        }
    }
}
</script>

<style scoped>
header {
    padding-bottom: 1px;

}

.navbar {
    font-weight: bold;
    padding: 40px 4%;
    font-size: 18px;
}

.nav-item-end {
    border-bottom: solid 1px red;
    padding-bottom: 10px;
}

.bi-list, .bi-x-lg {
    color: #FF0000;
}

.nav-link:hover {
    color: #FF0000 !important;
}
</style>