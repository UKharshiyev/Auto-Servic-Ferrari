<template>
    <div class="our-works" id="our-works">
        <h1 class="page-name text-light mb-4">Наши работы</h1>
        <div id="carouselExampleSlidesOnly" class="carousel slide d-none d-xl-block" data-bs-ride="carousel">
            <div class="carousel-inner">
                <div  v-for="(work, index) in worksName"
                      :key="index"
                      :class="index === 0 ? 'carousel-item active' : 'carousel-item' ">
                    <div class="row">
                        <div class="col-4">
                            <img src="../assets/img/Rectangle.png" class="d-block w-100" alt="...">
                            <div class="carousel-item-name text-center">
                                {{ work.name }}
                            </div>
                            <p>
                                {{work.text}}
                            </p>
                        </div>
                        <div class="col-4">
                            <img src="../assets/img/Rectangle.png" class="d-block w-100" alt="...">
                            <div class="carousel-item-name text-center">
                                {{ work.name }}
                            </div>
                            <p>
                                {{work.text}}
                            </p>
                        </div>
                        <div class="col-4">
                            <img src="../assets/img/Rectangle.png" class="d-block w-100" alt="...">
                            <div class="carousel-item-name text-center">
                                {{ work.name }}
                            </div>
                            <p>
                                {{work.text}}
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div id="carouselExampleSlidesOnly1" class="carousel slide d-none d-sm-block d-xl-none" data-bs-ride="carousel">
            <div class="carousel-inner">
                <div
                    v-for="(work, index) in worksName"
                    :key="index"
                    :class="index === 0 ? 'carousel-item active' : 'carousel-item' ">
                    <div class="row">
                        <div class="col-6">
                            <img src="../assets/img/Rectangle.png" class="d-block w-100" alt="...">
                            <div class="carousel-item-name text-center">
                                {{ work.name }}
                            </div>
                            <p>
                                {{work.text}}
                            </p>
                        </div>
                        <div class="col-6">
                            <img src="../assets/img/Rectangle.png" class="d-block w-100" alt="...">
                            <div class="carousel-item-name text-center">
                                {{ work.name }}
                            </div>
                            <p>
                                {{work.text}}
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div id="carouselExampleSlidesOnly2" class="carousel slide d-sm-none" data-bs-ride="carousel">
            <div class="carousel-inner">
                <div
                    v-for="(work, index) in worksName"
                    :key="index"
                    :class="index === 0 ? 'carousel-item active' : 'carousel-item'">
                    <img src="../assets/img/Rectangle.png" class="d-block w-100" alt="...">
                    <div class="carousel-item-name text-center">
                        {{ work.name }}
                    </div>
                    <p>
                        {{work.text}}
                    </p>
                </div>
            </div>
        </div>
        <div class=" d-none d-xl-block text-center">
           <button type="button" class="btn" data-bs-target="#carouselExampleSlidesOnly" data-bs-slide="prev">
               <img src="../assets/icons/prev-icon.png" class="d-block w-100 carousel-control-icon" alt="...">
           </button>
           <button type="button" class="btn" data-bs-target="#carouselExampleSlidesOnly" data-bs-slide="next">
               <img src="../assets/icons/next-icon.png" class="d-block w-100 carousel-control-icon" alt="...">
           </button>
       </div>
        <div class="d-none d-sm-block d-xl-none text-center">
            <button type="button" class="btn" data-bs-target="#carouselExampleSlidesOnly1" data-bs-slide="prev">
                <img src="../assets/icons/prev-icon.png" class="d-block w-100 carousel-control-icon" alt="...">
            </button>
            <button type="button" class="btn" data-bs-target="#carouselExampleSlidesOnly1" data-bs-slide="next">
                <img src="../assets/icons/next-icon.png" class="d-block w-100 carousel-control-icon" alt="...">
            </button>
        </div>
        <div class="d-sm-none text-center">
            <button type="button" class="btn" data-bs-target="#carouselExampleSlidesOnly2" data-bs-slide="prev">
                <img src="../assets/icons/prev-icon.png" class="d-block w-100 carousel-control-icon" alt="...">
            </button>
            <button type="button" class="btn" data-bs-target="#carouselExampleSlidesOnly2" data-bs-slide="next">
                <img src="../assets/icons/next-icon.png" class="d-block w-100 carousel-control-icon" alt="...">
            </button>
        </div>
        <h1 class="page-name text-light mt-4 mb-3" >Список моделей</h1>
        <div id="carouselExampleSlidesOnly3" class="carousel slide d-none d-xxl-block" data-bs-ride="carousel">
            <div class="carousel-inner">
                <div
                    v-for="(auto, index) in groupCarsByNumber(autoModels, 4)"
                    :key="index"
                    :class="index === 0 ? 'carousel-item active' : 'carousel-item'">
                    <div class="row">
                        <div
                            v-for="(autoItem, index) in auto"
                            :key="index"
                            class="col-3">
                            <div class="row listing-models mx-auto">
                                <div class="col-auto pe-0 pt-3">
                                    <div class="auto-model-img">
                                        <img :src="autoItem.urlImg" alt="...">
                                    </div>
                                </div>
                                <div class="col pt-3">
                                    <span class="model-name">
                                        {{ autoItem.name }}
                                    </span>
                                    <br/>
                                    <span class="text-light">
                                        {{ autoItem.year }}
                                    </span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div id="carouselExampleSlidesOnly4" class="carousel slide d-none d-xl-block d-xxl-none" data-bs-ride="carousel">
            <div class="carousel-inner">
                <div
                    v-for="(auto, index) in groupCarsByNumber(autoModels, 3)"
                    :key="index"
                    :class="index === 0 ? 'carousel-item active' : 'carousel-item'">
                    <div class="row">
                        <div
                            v-for="(autoItem, index) in auto"
                            :key="index"
                            class="col-4">
                            <div class="row listing-models mx-auto">
                                <div class="col-auto pe-0 pt-3">
                                    <div class="auto-model-img">
                                        <img :src="autoItem.urlImg" alt="...">
                                    </div>
                                </div>
                                <div class="col pt-3">
                                    <span class="model-name">
                                        {{ autoItem.name }}
                                    </span>
                                    <br/>
                                    <span class="text-light">
                                        {{ autoItem.year }}
                                    </span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div id="carouselExampleSlidesOnly5" class="carousel slide d-xl-none" data-bs-ride="carousel">
            <div class="carousel-inner">
                <div
                    v-for="(auto, index) in groupCarsByNumber(autoModels, 2)"
                    :key="index"
                    :class="index === 0 ? 'carousel-item active' : 'carousel-item'">
                    <div class="row">
                        <div class="col mt-3 pe-0 auto-first-model">
                            <div class="row listing-models mx-auto pt-3">
                                <div class="col px-0">
                                    <div class="auto-model-img">
                                        <img :src="auto[0].urlImg" alt="...">
                                    </div>
                                </div>
                                <div class="col auto-info">
                                    <span class="model-name">
                                        {{ auto[0].name }}
                                    </span>
                                    <br/>
                                    <span class="text-light model-year">
                                        {{ auto[0].year }}
                                    </span>
                                </div>
                            </div>
                        </div>
                        <div class="col mt-3 ps-0">
                            <div class="row listing-models mx-auto pt-3">
                                <div class="col px-0">
                                    <div class="auto-model-img">
                                        <img :src="auto[1].urlImg" alt="...">
                                    </div>
                                </div>
                                <div class="col auto-info">
                                    <span class="model-name">
                                        {{ auto[1].name }}
                                    </span>
                                    <br/>
                                    <span class="text-light model-year">
                                        {{ auto[1].year }}
                                    </span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class=" d-none d-none d-xxl-block text-center mt-4">
            <button type="button" class="btn" data-bs-target="#carouselExampleSlidesOnly3" data-bs-slide="prev">
                <img src="../assets/icons/prev-icon.png" class="d-block w-100 carousel-control-icon" alt="...">
            </button>
            <button type="button" class="btn" data-bs-target="#carouselExampleSlidesOnly3" data-bs-slide="next">
                <img src="../assets/icons/next-icon.png" class="d-block w-100 carousel-control-icon" alt="...">
            </button>
        </div>
        <div class="d-none d-xl-block d-xxl-none text-center mt-4">
            <button type="button" class="btn" data-bs-target="#carouselExampleSlidesOnly4" data-bs-slide="prev">
                <img src="../assets/icons/prev-icon.png" class="d-block w-100 carousel-control-icon" alt="...">
            </button>
            <button type="button" class="btn" data-bs-target="#carouselExampleSlidesOnly4" data-bs-slide="next">
                <img src="../assets/icons/next-icon.png" class="d-block w-100 carousel-control-icon" alt="...">
            </button>
        </div>
        <div class="d-xl-none text-center mt-4">
            <button type="button" class="btn" data-bs-target="#carouselExampleSlidesOnly5" data-bs-slide="prev">
                <img src="../assets/icons/prev-icon.png" class="d-block w-100 carousel-control-icon" alt="...">
            </button>
            <button type="button" class="btn" data-bs-target="#carouselExampleSlidesOnly5" data-bs-slide="next">
                <img src="../assets/icons/next-icon.png" class="d-block w-100 carousel-control-icon" alt="...">
            </button>
        </div>
    </div>
</template>

<script>
export default {
    name: "OurWorks",
    data() {
        return {
            worksName: [
                {name: "Название работы" , text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna"},
                {name: "Название работы" , text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna"},
                {name: "Название работы" , text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna"},
                {name: "Название работы" , text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna"},
            ],
            autoModels: [
                {name: "GTC4LUSSO", year: "2016-2020", urlImg: '/listing-models/listing-model-1.png'},
                {name: "PUROSANGUE", year: "2022", urlImg: '/listing-models/listing-model-2.png'},
                {name: "F8", year: "2019", urlImg: '/listing-models/listing-model-3.png'},
                {name: "812", year: "2017", urlImg: '/listing-models/listing-model-4.png'},
                {name: "GTC4LUSSO", year: "2016-2020", urlImg: '/listing-models/listing-model-1.png'},
                {name: "PUROSANGUE", year: "2022", urlImg: '/listing-models/listing-model-2.png'},
                {name: "F8", year: "2019", urlImg: '/listing-models/listing-model-3.png'},
                {name: "812", year: "2017", urlImg: '/listing-models/listing-model-4.png'},

            ]
        }
    },
    methods: {
        groupCarsByNumber(cars, num) {
            const groupedCars = [];
            const chunkSize = num;
            const numChunks = Math.ceil(cars.length / chunkSize);

            for (let i = 0; i < numChunks; i++) {
                groupedCars.push(cars.slice(i * chunkSize, (i + 1) * chunkSize));
            }

            return groupedCars;
        }
    },
}
</script>

<style scoped>
.our-works {
    margin: 0 4%;
    padding-bottom:  40px;
}

.page-name {
    font-size: 42px;
    font-weight: 800;
}

.carousel-item p {
    color: white;
    font-size: 20px;
    font-weight: 500;
}

.carousel-item-name {
    width: 100%;
    font-weight: 600;
    color: #FF0000;
    font-size: 22px;
}

.auto-model-img img {
    max-width: 116px;
}

.listing-models {
    font-weight: 600;
    width: 310px;
    height: 95px;
    border: 1px solid #FF0000;
    border-radius: 20px;
}

.model-name {
    color: #FF0000;
    font-size: 20px;
}

.carousel-control-icon {
    margin-top: -10px;
    width: 70% !important;
}

.carousel-item p {
    font-size: 14px;
}

@media screen and (max-width: 730px) {
    .model-name, .model-year {
        font-size: 12px;
    }

    .listing-models {
        width: 210px;
        height: 83px;
    }

    .auto-model-img img {
        max-width: 80px;
    }
}

@media screen and (max-width: 500px) {
    .page-name {
        font-size: 32px;
    }

    .carousel-control-icon {
        margin-top: -10px;
        width: 70% !important;
    }

    .carousel-item p {
        font-size: 14px;
    }

    .model-name {
        font-size: 10px;
    }

    .listing-models {
        width: 145px;
        height: 70px;
        padding-top: 10px !important;

    }

    .auto-model-img img {
        margin-top: 10px;
        width: 60px;
    }

    .auto-info {
        padding: 0;
    }
}

</style>