<template>
    <div class="our-service" id="our-service">
        <h1 class="page-name">Наши услуги</h1>
        <span class="the-service d-block">Снизу мы предоставили список наших услуг по разделам:</span>
        <div class="row our-service-container m-0">
            <div
                v-for="(content, index) in servicesImg"
                :key="index"
                class="our-service-content px-2 mb-2 col-6 col-md-4 col-lg-3"
            >
                <img :src="content.url" class="service-img" alt="img">
                <div class="service-name">
                    {{content.name}}
                </div>
            </div>
        </div>
        <div class="page-name page-title mt-4 mb-3" id="heading-benefits">
            Почему стоит выбрать нас
        </div>
        <div class="heading-benefits row">
            <div class="col-md-6 col-lg-4 mt-4">
                <img src="../assets/icons/cub.png">
                <div class="heading mt-2">
                    Заголовок преимущества
                </div>
                <p class="my-2">
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna
                </p>
            </div>
            <div class="col-md-6 col-lg-4 mt-4">
                <img src="../assets/icons/motor-icon.png">
                <div class="heading mt-2">
                    Заголовок преимущества
                </div>
                <p class="my-2">
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna
                </p>
            </div>
            <div class="col-md-6 col-lg-4 mt-4">
                <img src="../assets/icons/icon-time.png">
                <div class="heading mt-2">
                    Заголовок преимущества
                </div>
                <p class="my-2">
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna
                </p>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: "OurServices",
    data() {
        return {
            servicesImg: [
                {
                    url: '/img-service/img-1.png',
                    name: 'ТЕХ.ОБСЛУЖИВАНИЕ'
                },
                {
                    url: '/img-service/img-2.png',
                    name: 'ДИАГНОСТИКА'
                },
                {
                    url: '/img-service/img-3.png',
                    name: 'ХОДОВАЯ ЧАСТЬ'
                },
                {
                    url: '/img-service/img-4.png',
                    name: 'ТРАНСМИССИЯ'
                },
                {
                    url: '/img-service/img-5.png',
                    name: 'ДВИГАТЕЛЬ'
                },
                {
                    url: '/img-service/img-6.png',
                    name: 'ВЫХЛОПНАЯ\n' +
                        'СИСТЕМА'
                },
                {
                    url: '/img-service/img-7.png',
                    name: 'РУЛЕВОЕ УПРАВЛЕНИЕ'
                },
                {
                    url: '/img-service/img-8.png',
                    name: 'ТОПЛИВНАЯ СИСТЕМА'
                },
            ]
        }
    }
}
</script>


<style scoped>
.our-service {
    color: white;
    padding: 0 4% 40px;
    background-image: url("../assets/img/ferrari_logo_bg_icon.png");
    background-repeat: no-repeat;
    background-position: 0 30%;
    background-size: 210px;

}
.page-name {
    font-weight: 800;
    font-size: 32px;
}

.the-service {
    font-size: 15px;
    font-weight: 600;
    margin-bottom: 30px;
}

.service-img {
    width: 100%;
    border-radius: 10px;
}

.service-name {
    margin-top: 10px;
    font-size: 10px;
    font-weight: 600;
}

.heading-benefits img{
    width: 50px;
}

.heading {
    font-size: 18px !important;
    font-weight: 600;
}

.heading-benefits p {
    font-size: 17px;
}

@media screen and (max-width: 759px) {
    .page-title {
        font-size: 32px;
    }
}

@media screen and (min-width: 500px) {

    .service-name {
        font-size: 17px;
    }

    .the-service {
        font-size: 24px;
    }

    .heading-benefits img{
        width: 90px;
    }

    .page-name {
        font-size: 42px;
    }
}

</style>