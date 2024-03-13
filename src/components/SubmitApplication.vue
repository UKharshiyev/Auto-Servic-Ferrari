<template>
    <div class="submit-application-container position-relation">
        <h1 class="text-white submit-title">ПРЕВОСХОДСТВО В ОБСЛУЖИВАНИИ</h1>
        <h2 class="text-white submit-title-2 mt-4">Ваша машина в надежных руках!</h2>
        <img src="../assets/icons/bg-logo-icon.png" class="bg-logo-icon">
        <div class="container-img-auto">
            <img src="../assets/img/auto-1.png" class="auto-img-1">
        <span class="auto-name">
            F812 SUPER
        </span>
        </div>
        <button
            type="button"
            class="btn btn-lg btn-outline-danger submit-application-button"
            data-bs-toggle="modal"
            data-bs-target="#exampleModal"
        >
            ОСТАВИТЬ ЗАЯВКУ
        </button>
        <button type="button" class="btn btn-outline-warning ps-0 pt-0 mt-4 learn-button text-start d-block">
            <div class="row">
                <div class="col-3">
                    <img src="../assets/icons/italyIcon.png" class="auto-img-2">
                </div>
                <div class="col pt-2 text-white fw-bold">
                    Специально обученные механики
                </div>
            </div>
        </button>
        <button type="button" class="btn btn-outline-warning ps-0 pt-0 mt-4 learn-button text-start d-block">
            <div class="row">
                <div class="col-3">
                    <img src="../assets/icons/kingIcon.png" class="auto-img-3">
                </div>
                <div class="col pt-2 text-white fw-bold">
                    Только премиум качество
                </div>
            </div>
        </button>
        <div class="listing-down">
            <img src="../assets/icons/listing-down.png" class="listing-down-img me-3">
            Листайте вниз
        </div>
        <div class="submit-application px-1 px-2 px-sm-4 pt-4 text-light">
            <div>
                <span class="text-warning d-block">Чтобы узнать точную стоимость работ,</span>
                запишитесь на бесплатную консультацию
            </div>
            <div class="row mt-4">
                <div class="pe-0 col-12 col-md-6 col-lg-4">
                    <div class="input-group input-application">
                        <input type="text" class="form-control" placeholder="Ваше имя" aria-label="Recipient's username" aria-describedby="inputGroup-sizing-default">
                    </div>
                </div>
                <div class="py-2 pe-0 py-sm-0 col-12 col-md-6 col-lg-4 mt-3 mt-md-0">
                    <div class="input-group input-application">
                     <span class="input-group-text p-0" id="inputGroup-sizing-default">
                                <div class="dropdown">
                                        <button class="btn border-0" type="button" data-bs-toggle="dropdown" aria-expanded="false">
                                              <img src="../assets/icons/russia.png" class="me-2">
                                              <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="currentColor" class="bi bi-chevron-down mt-1" viewBox="0 0 16 16">
                                                  <path fill-rule="evenodd" d="M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708"/>
                                              </svg>
                                        </button>
                                      <ul class="dropdown-menu dropdown-menu-dark">
                                        <li><a class="dropdown-item active" href="#">RU</a></li>
                                        <li><a class="dropdown-item" href="#">UZ</a></li>
                                        <li><a class="dropdown-item" href="#">ENG</a></li>
                                      </ul>
                                </div>
                            </span>
                        <input type="text" placeholder="+7 (999) 999-99-99" class="form-control" aria-label="Sizing example input" aria-describedby="inputGroup-sizing-default">
                    </div>
                </div>
                <div class="col-12 col-lg-4 pe-0 mt-3 mt-lg-0">
                   <div>
                       <button
                           type="button"
                           class="btn  form-control submit-application-btn"
                       >
                           ЗАПИСАТЬСЯ
                       </button>
                   </div>
                </div>
            </div>
            <p>
                Оставляя заявку, вы даете согласие на обработку персональных данных
            </p>
        </div>
    </div>
    <!-- Modal -->
    <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content px-4">
                <img src="../assets/icons/bg-logo-icon-original.png" class="modal-bg-img">
                <div class="text-end">
                    <button type="button" class="close-btn" data-bs-dismiss="modal" aria-label="Close">
                        <svg xmlns="http://www.w3.org/2000/svg" width="40" height="40" fill="currentColor" class="bi bi-x-lg" viewBox="0 0 16 16">
                            <path d="M2.146 2.854a.5.5 0 1 1 .708-.708L8 7.293l5.146-5.147a.5.5 0 0 1 .708.708L8.707 8l5.147 5.146a.5.5 0 0 1-.708.708L8 8.707l-5.146 5.147a.5.5 0 0 1-.708-.708L7.293 8z"/>
                        </svg>
                    </button>
                </div>
                <div>
                    <h1 class="modal-title">Оставьте заявку</h1>
                    <p>Заполните форму и мы Вам перезвоним!</p>
                    <div class="input-group">
                            <span class="input-group-text p-0" id="inputGroup-sizing-default">
                                <div class="dropdown">
                                        <button class="btn border-0" type="button" data-bs-toggle="dropdown" aria-expanded="false">
                                              <img src="../assets/icons/russia.png" class="me-2">
                                              <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="currentColor" class="bi bi-chevron-down mt-1" viewBox="0 0 16 16">
                                                  <path fill-rule="evenodd" d="M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708"/>
                                              </svg>
                                        </button>
                                      <ul class="dropdown-menu dropdown-menu-dark">
                                        <li><a class="dropdown-item active" href="#">RU</a></li>
                                        <li><a class="dropdown-item" href="#">UZ</a></li>
                                        <li><a class="dropdown-item" href="#">ENG</a></li>
                                      </ul>
                                </div>
                            </span>
                        <input type="text" placeholder="+7 (999) 999-99-99" class="form-control" aria-label="Sizing example input" aria-describedby="inputGroup-sizing-default">
                    </div>
                    <div class="my-3">
                        <button type="button" class="btn send-button py-2">
                            ОТПРАВИТЬ
                        </button>
                    </div>
                    <p>Оставляя заявку, вы даете согласие на обработку персональных данных</p>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "SubmitApplication"
}
</script>

<style scoped>
.submit-application-container {
    padding: 50px 0 0 4% ;
}

.auto-img-1 {
    margin-left: 30%;
    width: 65%;
    filter: drop-shadow(0 0 0.90rem #FF0000);
    position: absolute;
    z-index: 2;
}

.bg-logo-icon {
    position: absolute;
    right: 0;
    bottom: 14%;
    z-index: 1;
}

.submit-title {
    font-family: "Montserrat ExtraBold";
}

.submit-title-2 {
    margin-bottom: 40px;
}

.submit-application-button {
    margin: 65px 0 65px;
    height: 61px;
    width: 300px;
    color: white;
    background: #FF0000;
}

.learn-button {
    width: 300px;
    height: 61px;
    border-radius: 40px 10px 10px 40px;
}

.learn-button img {
    margin-left: -2px;
}

.auto-name {
    right: 9%;
    top: 44%;
    font-size: 100px;
    position: absolute;
    z-index: 1;
    font-weight: 800;
    color: white;
}

.listing-down {
    padding: 100px 0 60px;
    color: white;
    font-weight: 600;
    font-size: 22px;
}

.modal-content {
    background: rgb(26, 26, 26);
    border-radius: 10px;
    border-color: #FF0000;
    color: white;
    position: relative;
    padding: 16px 0;
    text-align: center;
}

.close-btn {
    background: rgb(26, 26, 26);
    border: none;
    color: #FF0000;
    font-weight: 600;
}

.modal-title {
    font-size: 42px;
    font-weight: 800;
}

.modal-bg-img {
    position: absolute;
    width: 70%;
    top:50%;
    left:50%;
    transform:translate(-50%, -50%);
    z-index: 1;
}

.modal-content p {
    font-size: 21px;
    font-weight: 600;
}

.modal-content .input-group {
    position: relative;
    z-index: 2;
}

.send-button {
    width: 100%;
    background: #FF0000;
    font-weight: 600;
    color: white;
    position: relative;
    z-index: 1;
}

.bi-chevron-down {
    color: #FF0000;
}
.dropdown-menu-dark li {
    z-index: 2;
}

.submit-application {
    margin-right: 4%;
    border: 1px solid #FF0000;
    border-radius: 10px;
    font-size: 30px;
    background-image: url("../assets/img/aplication-bg.png");
    background-repeat: no-repeat;
    background-position: right;
    background-color: #1A1A1A;

}

.form-control, #inputGroup-sizing-default, input, .submit-application-btn{
    height: 43px;
}
.submit-application-btn {
    background-color: #FF0000;
    color: white;
    margin-bottom: 6px;
    max-width: 280px;
}

.input-application {
    max-width: 400px;
}

.submit-application p {
    margin-top: 20px;
    font-size: 13px;
}
@media screen and (max-width: 1000px) {
    .auto-img-1 {
        margin-left: 0;
        width: 100%;
        position: relative;
    }

    .container-img-auto {
        position: relative;
    }
    .auto-name {
        font-size: 94px;
        top: -20%;
        position: absolute;
    }

    .submit-title {
        font-size: 30px;
    }

    .submit-application {
        font-size: 20px;
    }
}

@media screen and (max-width: 720px) {
    .submit-title-2 {
        font-size: 22px;
    }

    .submit-title {
        font-size: 22px;
    }

    .bg-logo-icon {
        bottom: 25%;
    }


    .auto-name {
        font-size: 64px;
        top: -20%;
    }

    .modal-title {
        font-size: 20px;
    }

    .modal-content p {
        font-size: 14px;
    }

    .submit-application {
        font-size: 18px;
    }
}


@media screen and (max-width: 480px) {
    .submit-title-2 {
        font-size: 16px;
    }

    .submit-title {
        font-size: 15px;
    }
    .learn-button {
        width: 96%;
    }
    .submit-application-button {
        width: 96%;
    }

    .auto-name {
        font-size: 45px;
        top: -20%;
    }

    .close-btn svg {
        width: 30px;
        height: 30px;
    }

    .submit-application div {
        font-size: 14px;
    }

    .input-application {
        max-width: 280px;
    }
}
</style>