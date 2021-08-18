<template>
<section class="blog" id="blog">
    <div class="container">
        <div class="blog-discr">
            <h2 class="general-title">
                Blog
            </h2>
            <p class="general-subtitle">
                Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                Inventore id laborum deserunt sequi saepe repellendus provident.
                Consequatur cupiditate aliquam accusantium sed,
                ipsa dolorem rerum odio eaque, saepe earum error numquam.
            </p>
        </div>
        <div class="blog-main">
            <div class="blog-main__content blog-main__content--first-post">
                <div class="blog-main__content-date">
                    <span class="blog-main__content-date-number">
                        20
                    </span>
                    <span class="blog-main__content-date-mounth">
                        nov
                    </span>
                </div>
                <div class="blog-main__content-name">
                    <a href="#" class="blog-main__content-link">
                        <h3 class="blog-main__content-title">
                        Green Smoothies: Too Much of a Good Thing?
                        </h3>
                    </a>
                    <span class="blog-main__content-author">
                        By Auskteez - 2 hours ago
                    </span>
                </div>
            </div>
            <div class="blog-main__content blog-main__content--second-post">
                <div class="blog-main__content-date">
                    <span class="blog-main__content-date-number">
                        14
                    </span>
                    <span class="blog-main__content-date-mounth">
                        nov
                    </span>
                </div>
                <div class="blog-main__content-name">
                    <a href="#" class="blog-main__content-link">
                        <h3 class="blog-main__content-title">
                        Growing Food and a “Thirst” for Innovation
                        </h3>
                    </a>
                    <span class="blog-main__content-author">
                        By Auskteez - 3 hours ago
                    </span>
                </div>
            </div>
            <div class="blog-main__content blog-main__content--third-post">
                <div class="blog-main__content-date">
                    <span class="blog-main__content-date-number">
                        10
                    </span>
                    <span class="blog-main__content-date-mounth">
                        nov
                    </span>
                </div>
                <div class="blog-main__content-name">
                    <a href="#" class="blog-main__content-link">
                        <h3 class="blog-main__content-title">
                        Pesticides & Food: What You Need to Know
                        </h3>
                    </a>
                    <span class="blog-main__content-author">
                        By Auskteez - 6 hours ago
                    </span>
                </div>
            </div>
        </div>
        <div class="general-button blog-button">
            <button class="general-button__btn blog-button__btn">
                view more
            </button>
        </div>
    </div>
</section>
</template>

<script>
export default {
  name: 'Blog',
};
</script>

<style lang="scss">
.blog {
    background: #b07cf7;
    color: #ffffff;
    padding: 100px 0;

    &-discr {
        width: 50%;
        margin: 0 auto 40px;
    }

    &-main {
        display: flex;
        align-items: center;
        justify-content: space-between;

        &__content {
            padding: 30px;
            width: 370px;
            height: 310px;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            box-shadow: 12px -158px 75px -41px rgba(0,0,0,0.9) inset;

            &:hover {
                filter: drop-shadow(3px 0px 15px #000000);
                transition-duration: 0.5s;
            }
        }

        &__content--first-post {
            background-image: url("~@/assets/image/blog/img_1.png");
        }

        &__content--second-post {
            background-image: url("~@/assets/image/blog/img_2.png");
            background-position: bottom;
        }

        &__content--third-post {
            background-image: url("~@/assets/image/blog/img-3.png");
            background-position: center;
        }

        &__content-date {
            display: flex;
            flex-direction: column;
            width: fit-content;
            background: rgba(0,0,0,0.40);
            border-radius: 10%;

            &-number {
                text-align: center;
                font-family: 'ralewaybold', sans-serif;
                font-weight: 700;
                font-size: 32px;
                margin-top: -5px;
                margin-bottom: -10px;
                padding: 0 15px;
            }

            &-mounth {
                text-align: center;
                font-family: 'ralewayheavy', sans-serif;
                font-weight: 900;
                font-size: 21px;
                text-transform: uppercase;
            }
        }

        &__content-link {
            text-decoration: none;
            color: #ffffff;

            &:hover {
                color: #b07cf7;
                transition-duration: 0.5s;
            }
        }

        &__content-title {
            font-family: 'ralewaybold', sans-serif;
            font-weight: 700;
            font-size: 20px;
        }

        &__content-author {
            font-family: 'ralewaylight', sans-serif;
            font-weight: 300;
            font-size: 13px;
        }
    }

    &-button {
        margin-top: 50px;

        &__btn {
            background: #f72a3b;
            padding: 10px 40px;
        }
    }
}

@media screen and (max-width: 1400px) {
    .blog {
        &-main__content {
            margin: 0 20px;
        }
    }
}

@media screen and (max-width: 1200px) {
    .blog {
        &-discr {
            width: 70%;
        }

        &-main {
            flex-wrap: wrap;
            justify-content: center;

            &__content {
                margin-top: 40px;
            }
        }
    }
}

@media screen and (max-width: 768px) {
    .blog {
        &-discr {
            width: 100%;
        }
    }
}
</style>
