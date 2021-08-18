<template>
<section class="gallery" id="gallery">
    <div class="container">
        <div class="gallery-discr">
            <h2 class="general-title">
                Gallery
            </h2>
            <p class="general-subtitle">
                Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                Inventore id laborum deserunt sequi saepe repellendus provident.
                Consequatur cupiditate aliquam accusantium sed,
                ipsa dolorem rerum odio eaque, saepe earum error numquam.
            </p>
        </div>
        <div class="gallery-main">
            <div class="gallery-main__top">
                <img class="gallery-main__img"
                src="~@/assets/image/gallery/peaches.png"
                alt="peaches" width="778px" height="550px">
                <div class="gallery-main__col">
                    <img class="gallery-main__img"
                    src="~@/assets/image/gallery/blueberry.png"
                    alt="blueberry" width="370px" height="260px">
                    <img class="gallery-main__img"
                    src="~@/assets/image/gallery/blackberry.png"
                    alt="blackberry" width="370px" height="260px">
                </div>
            </div>
            <div class="gallery-main__bottom">
                <img class="gallery-main__img"
                src="~@/assets/image/gallery/cream.png"
                alt="cream" width="570px" height="400px">
                <img class="gallery-main__img"
                src="~@/assets/image/gallery/persimmon.png"
                alt="persimmon" width="570px" height="400px">
            </div>
        </div>
        <div class="general-button gallery-button">
            <button class="general-button__btn gallery-button__btn">
                view more
            </button>
        </div>
    </div>
</section>
</template>

<script>
export default {
  name: 'Gallery',
};
</script>

<style lang="scss">
.gallery {
    background: #ffe92f;
    color: #262626;
    padding: 80px 0 110px 0;

    .container {
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    &-discr {
        text-align: center;
        width: 50%;
        margin: 0 auto 40px;
    }

    &-main {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;

        &__img {
            margin: 10px;
        }

        &__top {
            display: flex;
        }

        &__col {
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }
    }

    &-button {
        margin-top: 50px;

        &__btn {
            background: #5585a2;
            padding: 10px 40px;
        }
    }
}

@media screen and (max-width: 1400px) {
    .gallery {

        &-main__top {
            flex-wrap: wrap;
            justify-content: center;
        }

        &-main__col {
            flex-direction: row;

            .gallery-main__img {
                margin: 20px;
            }
        }

        &-main__bottom {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }
    }
}

@media screen and (max-width: 768px) {
    .gallery {

        &-discr {
            width: 100%;
        }

        &-main {
            justify-content: center;

            &__top {

                .gallery-main__img {
                    width: 100%;
                    height: auto;
                }
            }

            &__col {
                flex-direction: column;
                align-items: center;
            }

            &__bottom {
                .gallery-main__img {
                    width: 100%;
                    height: auto;
                }
            }
        }
    }
}
</style>
