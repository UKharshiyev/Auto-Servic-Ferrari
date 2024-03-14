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
        <div class="page-name page-title mt-4 mb-3">
            Почему стоит выбрать нас
        </div>
        <div class="heading-benefits row ">
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
                    url: 'img-service/img-1.png',
                    name: 'ТЕХ.ОБСЛУЖИВАНИЕ'
                },
                {
                    url: 'img-service/img-1.png',
                    name: 'ТЕХ.ОБСЛУЖИВАНИЕ'
                },
                {
                    url: 'img-service/img-1.png',
                    name: 'ТЕХ.ОБСЛУЖИВАНИЕ'
                },
                {
                    url: 'img-service/img-1.png',
                    name: 'ВЫХЛОПНАЯ\n' +
                        'СИСТЕМА'
                },
                {
                    url: 'img-service/img-1.png',
                    name: 'ТЕХ.ОБСЛУЖИВАНИЕ'
                },
                {
                    url: 'img-service/img-1.png',
                    name: 'ТЕХ.ОБСЛУЖИВАНИЕ'
                },
            ]
        }
    }
}
</script>


<style scoped>
.our-service {
    color: white;
    margin: 0 4%;
    padding-bottom:  40px;
}
.page-name {
    font-size: 21px;
    font-weight: 800;

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
.page-name {
    font-size: 32px;
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