<template>
    <div class="row mt-5 pb-5 mx-0 footer-container">
        <div class="col-7 col-lg-10 px-0">
            <div class="row">
				<div class="col-md-8 col-lg-4 col-xxl-3">
					<img src="../assets/icons/ferrari-text-icon.png" width="170" class="footer-ferrari-icon d-block">
					<span class="footer-copy d-block">
                        © 2023 Company name
                    </span>
					<span class="footer-copy d-block mt-1 mb-md-0">
                        Все права защищены
					</span>
					<div class="footer-conf-text mt-1 mb-4">
						<span>
							Политика конфиденциальности
						</span>
					</div>
                </div>
				<div class="col footer-links d-lg-flex justify-content-lg-around">
					<a href="#our-service" class="d-block"><span>Услуги</span></a>
					<a href="#heading-benefits" class="d-block"><span>Преимущества</span></a>
					<a href="#our-works" class="d-block"><span>Наши работы</span></a>
					<a href="#contacts" class="d-block"><span>Контакты</span></a>
				</div>
            </div>
        </div>
        <div class="col-5 col-lg-2">
            <a href="#navbar" class="up-listing-icon d-block text-end">
                <img src="../assets/icons/up-listing-icon.png" width="32">
                Наверх
            </a>
        </div>
    </div>
</template>

<script>
export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: "Footer"
}
</script>

<style scoped>
.footer-container {
    padding: 0 4%;
	background: linear-gradient(#1A1A1A, #333333);
}

.footer-copy {
    margin-top: 20px;
    color: white;
    font-weight: 500;
}

.up-listing-icon {
    color: white;
    font-weight: 600;
    text-decoration: none;
    font-size: 18px;
}

.footer-links a {
	font-size: 18px;
	font-weight: 600;
	color: white;
	text-decoration: none;
}

.footer-links a span:hover, .up-listing-icon:hover {
	color: #FF0000;
}

.footer-conf-text {
	height: 16px;
}

.footer-conf-text span {
	color: white;
	font-weight: 500;
	position: absolute;
}

@media screen and (max-width: 500px) {
	.footer-copy, .footer-conf-text span {
		font-size: 14px;
	}
	
	.footer-ferrari-icon {
		width: 130px;
	}
	
	.up-listing-icon, .footer-links {
		font-size: 15px;
	}
	
	.up-listing-icon img {
		width: 24px;
	}
}
</style>