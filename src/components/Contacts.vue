<template>
    <div class="row contacts-container mx-0" id="contacts">
        <div class="col-12 col-lg-6">
            <h1 class="page-name text-light pb-4">Контакты</h1>
            <div class="row">
                <div class="col-1">
                    <img src="../assets/icons/placeholder.png" width="35" class="contact-icon">
                </div>
                <div class="col-11">
                    <div class="contact-content">
                        Наш адрес:
                    </div>
                    <span class="content-text">Россия, г. Москва, улица Пушкина, дом 1, корпус 2</span>
                </div>
            </div>
            <div class="row my-3">
                <div class="col-1">
                    <img src="../assets/icons/phone-call.png" width="35" class="contact-icon">
                </div>
                <div class="col-11">
                    <div class="contact-content">
                        Номер телефона:
                    </div>
                    <span class="content-text">+7 (999) 999-09-90</span>
                </div>
            </div>
            <div class="row mb-3">
                <div class="col-1">
                    <img src="../assets/icons/mail.png" width="35" class="contact-icon">
                </div>
                <div class="col-11">
                    <div class="contact-content">
                        Наш E-mail:
                    </div>
                    <span class="content-text">example.email@gmail.com</span>
                </div>
            </div>
            <div class="submit-app-title-child">
                Мы в социальных сетях
            </div>
            <div class="mb-4 mt-2">
                <img src="../assets/icons/whatsapp-icon.png" width="35" class="contact-icon me-4">
                <img src="../assets/icons/telegram-icon.png" width="35" class="contact-icon">
            </div>
        </div>
        <div class="col-12 col-lg-6 mb-4 mt-lg-0 mt-4">
            <div class="submit-app px-1">
                <div class="submit-app-title">Оставьте заявку</div>
                <p class="submit-app-title-child">
                    Заполните форму и мы Вам перезвоним!
                </p>
                <div class="input-group input-application mx-auto px-1">
                    <input type="text" class="form-control" placeholder="Ваше имя" aria-label="Recipient's username" aria-describedby="inputGroup-sizing-default">
                </div>
                <div class="input-group input-application mx-auto my-3 px-1">
                     <span class="input-group-text p-0" id="inputGroup-sizing-default">
                         <div class="dropdown">
                             <button class="btn border-0" type="button" data-bs-toggle="dropdown" aria-expanded="false">
                                 <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24"
                                      fill="currentColor" class="bi bi-chevron-down mt-1"
                                      viewBox="0 0 16 16">
                                        <path fill-rule="evenodd" d="M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708"/>
                                 </svg>
                             </button>
                             <ul class="dropdown-menu dropdown-menu-dark">
                                 <li><a class="dropdown-item active" href="#">1</a></li>
                                 <li><a class="dropdown-item" href="#">2</a></li>
                                 <li><a class="dropdown-item" href="#">3</a></li>
                             </ul>
                         </div>
                     </span>
                    <input type="text" placeholder="Выберите интересующую услугу" class="form-control form-control-service" aria-label="Sizing example input" aria-describedby="inputGroup-sizing-default">
                </div>
                <div class="input-group input-application mx-auto px-1 mb-3">
                     <span class="input-group-text p-0" id="inputGroup-sizing-default">
                         <div class="dropdown">
                             <button class="btn border-0" type="button" data-bs-toggle="dropdown" aria-expanded="false">
                                 <img src="../assets/icons/russia.png" class="me-2">
                                 <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24"
                                    fill="currentColor" class="bi bi-chevron-down mt-1"
                                    viewBox="0 0 16 16">
                                        <path fill-rule="evenodd"
                                        d="M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708"/>
                                 </svg>
                             </button>
                             <ul class="dropdown-menu dropdown-menu-dark">
                                 <li><a class="dropdown-item active" href="#">RU</a></li>
                                 <li><a class="dropdown-item" href="#">UZ</a></li>
                                 <li><a class="dropdown-item" href="#">ENG</a></li>
                             </ul>
                         </div>
                     </span>
                    <input type="text" placeholder="+7 (999) 999-99-99" class="form-control form-control-service" aria-label="Sizing example input" aria-describedby="inputGroup-sizing-default">
                </div>
                <p class="submit-app-title-child">
                    Оставляя заявку, вы даете согласие на обработку персональных данных
                </p>
                <div>
                    <button
                        type="button"
                        class="btn form-control submit-application-btn"
                    >
                        ЗАПИСАТЬСЯ
                    </button>
                </div>
            </div>
        </div>
    </div>
    <div id="container" class="mt-4"></div>
</template>

<script>
import { load } from '@2gis/mapgl';
export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: "Contacts",
    mounted() {
        load().then((mapglAPI) => {
            let map = new mapglAPI.Map('container', {
                center: [37.592631, 55.742371],
                zoom: 12,
                key: "912e999f-1634-437f-bca1-a422fc33dcb6",
            });

            new mapglAPI.Marker(map, {
                coordinates: [37.592631, 55.742371],
                icon: '/location-icon.png',
                size: [35, 70]
            });
        });
    }
}
</script>


<style scoped>
.contacts-container {
    padding: 0 4%;
}

.page-name {
    font-weight: 800;
    font-size: 42px;
}

.submit-app {
    border: solid 1px #FF0000;
    filter: drop-shadow(0 0 12mm #FF0000);
    border-radius: 20px;
    text-align: center;
    padding: 30px 0;
    background: #242424;
}

.submit-app-title {
    font-weight: 800;
    color: white;
    font-size: 42px;
}

.submit-app-title-child {
    color: white;
    font-weight: 600;
    font-size: 20px;
}

.bi-chevron-down {
    color: #FF0000;
}
.dropdown-menu-dark li {
    z-index: 2;
}

.form-control, #inputGroup-sizing-default, input, .submit-application-btn{
    height: 43px;
}
.submit-application-btn {
    font-weight: 600;
    background-color: #FF0000;
    color: white;
    margin-bottom: 6px;
    max-width: 280px;
}

.input-application {
    max-width: 400px;
}

.contact-content {
    font-weight: 600;
    color: white;

}

.content-text {
    color: white;
    display: block;
}

#container {
    width: 100%;
    height: 400px;
}

@media screen and (max-width: 500px) {
    #container {
        height: 260px;
    }

    .page-name{
        font-size: 32px;
    }

    .submit-app-title {
        font-size: 28px;
    }

    .submit-app-title-child {
        font-size: 16px;
    }

    .form-control-service {
        font-size: 12px;
        padding: 6px 0 6px 1px;
    }

    .submit-app {
        filter: drop-shadow(0 0 4mm #FF0000);
    }

    .contact-icon {
        width: 22px;
    }

    .contact-content, .content-text {
        padding-left: 5px;
    }
}
</style>