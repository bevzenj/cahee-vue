<template>
<section class="services" id="services">
    <div class="container">
        <div class="services-content">
            <div class="services-content__block">
                <div class="services-content__block-title">
                    Online Shopping
                </div>
                <div class="services-content__block-icon">
                    1
                </div>
            </div>
            <div class="services-content__block">
                <div class="services-content__block-title">
                    Quality Product
                </div>
                <div class="services-content__block-icon">
                    2
                </div>
            </div>
            <div class="services-content__block">
                <div class="services-content__block-title">
                    Domestic & International Delivery
                </div>
                <div class="services-content__block-icon">
                    3
                </div>
            </div>
            <div class="services-content__block">
                <div class="services-content__block-title">
                    Well Organized
                </div>
                <div class="services-content__block-icon">
                    4
                </div>
            </div>
        </div>
        <div class="services-name">
            <img class="services-name__img"
            src="~@/assets/image/services/tomatoes.png" alt="tomatoes">
            <div class="general-title services-name__title">
                Our Services
            </div>
        </div>
    </div>
</section>
</template>

<script>

export default {
  name: 'Services',
};
</script>

<style lang="scss">
.services {
    background-color: #70bfff;
    padding: 150px 0;
    position: relative;

    .container {
        display: flex;
        justify-content: space-between;
    }

    &-content {
        width: 40%;
    }

    &-content__block {
        display: flex;
        justify-content: space-between;
        align-items: center;
        background: #ffffff;
        height: 100px;
        margin-top: 20px;
        box-shadow: 4px 4px 10px 0px rgba(0,0,0,0.5);

        &:hover,
        &#icon {
            background: none;
            color: #ffffff;
            fill: #ffffff;
            transition-duration: 0.5s;
        }

        &-title {
            font-family: 'ralewaybold', sans-serif;
            font-weight: 700;
            font-size: 20px;
            text-align: center;
            width: 300px;
        }

        &-icon {
            display: flex;
            justify-content: center;
            align-items: center;
            width: 100px;
            height: 100%;
            position: relative;

            &::before {
                content: "";
                height: 100%;
                width: 1px;
                background: #9d9d9d;
                position: absolute;
                left: 0;
            }
        }
    }

    &-name {
        display: flex;
        align-items: center;
        width: 40%;

        &__img {
            position: absolute;
        }

        &__title {
            position: relative;
            color: #ffffff;
        }
    }
}

@media screen and (max-width: 1200px) {
    .services {
        &-name__img {
            width: 30%;
        }
    }
}

@media screen and (max-width: 992px) {
    .services {

        .container {
            flex-direction: column;
            align-items: center;
        }

        &-content {
            order: 2;
            width: 70%;
        }

        &-name {
            order: 1;
            text-align: center;

            &__img {
                display: none;
            }
        }
    }
}

@media screen and (max-width: 768px) {
    .services {

        &-content {
            width: 80%;
        }

        &-name {
            width: 100%;
        }
    }
}

@media screen and (max-width: 768px) {
    .services {
        &-name {
            display: block;
        }
    }
}
</style>
