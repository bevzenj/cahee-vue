<template>
<section class="about" id="about">
    <div class="container">
        <div class="">
            <img class="about__img" src="~@/assets//image/about/cup.png" alt="">
        </div>
        <div class="about-content">
            <h2 class="about__title general-title">
                About Us
            </h2>
            <div class="about__text">
                <p>
                    Abore Cahee magna aliqua. Ut enim ad minim veniam,
                    quis nostrud exercitation ullamco laboris nisi ut aliquip ex commodo consequat.
                    Duis aute irure dolor in reprehenderit in voluptate velit esse cillum.
                </p>
                <p>
                    Nim id est laborum. Sed ut perspiciatis unde omnis iste natus error
                    sit voluptatem accusantium doloremque laudantium,
                    totam rem aperiam, eaque ipsa quae ab illo inventore.
                </p>
            </div>
        </div>
    </div>
</section>
</template>

<script>

export default {
  name: 'About',
};
</script>

<style lang="scss">
.about {
    background: #00c3c3;
    margin-top: -60px;
    color: #ffffff;

    .container {
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 20px 0;
    }

    &-content {
        width: 40%;
    }

    &__img {
        width: 100%;
    }

    &__title {
       text-align: left
    }

    &__text {
        font-family: 'ralewaylight', sans-serif;
        font-weight: 300;
        font-size: 17px;

        &> p {
            margin-bottom: 20px;
        }
    }
}

@media screen and (max-width: 768px) {
    .about {
        &__img {
            display: none;
        }

        &-content {
            width: 100%;
            margin: 200px 20px;
        }
    }
}
</style>
