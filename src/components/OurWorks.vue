<template>
    <div class="our-works" id="our-works">
        <h1 class="page-name text-light mb-4">Наши работы</h1>
        <div id="carouselExampleRide" class="carousel slide d-none d-xl-block" data-bs-ride="true">
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
        <div id="carouselExampleRide1" class="carousel slide d-none d-sm-block d-xl-none" data-bs-ride="true">
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
        <div id="carouselExampleRide2" class="carousel slide d-sm-none" data-bs-ride="true">
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
           <button type="button" class="btn" data-bs-target="#carouselExampleRide" data-bs-slide="prev">
               <img src="../assets/icons/prev-icon.png" class="d-block w-100 carousel-control-icon" alt="...">
           </button>
           <button type="button" class="btn" data-bs-target="#carouselExampleRide" data-bs-slide="next">
               <img src="../assets/icons/next-icon.png" class="d-block w-100 carousel-control-icon" alt="...">
           </button>
       </div>
        <div class="d-none d-sm-block d-xl-none text-center">
            <button type="button" class="btn" data-bs-target="#carouselExampleRide1" data-bs-slide="prev">
                <img src="../assets/icons/prev-icon.png" class="d-block w-100 carousel-control-icon" alt="...">
            </button>
            <button type="button" class="btn" data-bs-target="#carouselExampleRide1" data-bs-slide="next">
                <img src="../assets/icons/next-icon.png" class="d-block w-100 carousel-control-icon" alt="...">
            </button>
        </div>
        <div class="d-sm-none text-center">
            <button type="button" class="btn" data-bs-target="#carouselExampleRide2" data-bs-slide="prev">
                <img src="../assets/icons/prev-icon.png" class="d-block w-100 carousel-control-icon" alt="...">
            </button>
            <button type="button" class="btn" data-bs-target="#carouselExampleRide2" data-bs-slide="next">
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
            ]
        }
    }
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
}
</style>