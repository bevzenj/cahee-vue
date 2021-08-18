<template>
<section class="contact" id="contact">
    <div class="container">
        <div class="contact-header">
            <h2 class="general-title">
                Contact
            </h2>
            <p class="general-subtitle">
                For new projects, ideas, business or anything
                you'd like to discuss, contact with me!
            </p>
        </div>
        <div class="contact-main">
            <form class="contact-main__form" action="" method="get">
                <input class="contact-main__form-input"
                type="text" id="username"
                name="username" placeholder="Your name..">
                <input class="contact-main__form-input"
                type="email" id="useremail"
                name="useremail" placeholder="Your email..">
                <input class="contact-main__form-input"
                type="tel" id="userphone" name="userphone"
                placeholder="Your phone number..">
                <textarea class="contact-main__form-input"
                name="textarea" id="textarea"
                cols="30" rows="10" placeholder="Your massage.."></textarea>
            </form>
            <div class="contact-main__info">
                <div class="contact-main__info-block">
                    <h4 class="contact-main__info-title">
                        address
                    </h4>
                    <address class="contact-main__info-discr">
                        123 City name, Street, City, Country
                    </address>
                </div>
                <div class="contact-main__info-block">
                    <h4 class="contact-main__info-title">
                        email
                    </h4>
                    <a class="contact-main__info-discr
                    contact-main__info-discr--link"
                    href="malito:cahee@domain.com">
                        cahee@domain.com
                    </a>
                </div>
                <div class="contact-main__info-block">
                    <h4 class="contact-main__info-title">
                        phone
                    </h4>
                    <a class="contact-main__info-discr
                    contact-main__info-discr--link"
                    href="tel:+0123456789">
                        +012 345 6789
                    </a>
                </div>
            </div>
        </div>
    </div>
</section>
</template>

<script>
export default {
  name: 'Contact',
};
</script>

<style lang="scss">
.contact {
    background: url('~@/assets//image/contact/background_contact.png');
    background-size: 100%;
    background-repeat: no-repeat;
    background-position: center center;
    background-attachment: fixed;
    background-size: cover;
    height: 100%;
    color: #262626;

    &-header {
        margin: 0 auto;
        text-align: center;
        padding-top: 90px;
        width: 30%;
    }

    &-main {
        display: flex;
        justify-content: space-between;
        margin-top: 50px;
        padding-bottom: 120px;

        &__form {
            width: 40%;
        }

        &__form-input {
            display: flex;
            flex-direction: column;
            width: 100%;
            background: rgba(0,196,196,0.5);
            outline: none;
            border: none;
            color: #ffffff;
            padding: 20px 15px;
            margin-bottom: 15px;

            &::placeholder {
                font-size: 17px;
                color: rgba(255,255,255,0.7);;
            }

            &:focus {
                border-left: 5px solid #262626;
                transition-duration: 0.2s;
                background: rgba(0,196,196,1);
            }
        }

        &__info {
            width: 50%;

            &-block {
                margin-top: 20px;
            }
        }

        &__info-title {
            font-family: 'ralewaybold', sans-serif;
            font-weight: 700;
            font-size: 17px;
            text-transform: uppercase;
        }

        &__info-discr {
            font-family: 'ralewaylight', sans-serif;
            font-weight: 300;
            font-size: 20px;

            &--link {
                text-decoration: none;
                color: inherit;
            }
        }
    }
}

@media screen and (max-width: 1200px) {
    .contact {
        &-header {
            width: 50%;
        }
    }
}

@media screen and (max-width: 992px) {
    .contact {

        &-header {
            width: 100%;
        }

        &-main {
            flex-direction: column;

            &__form {
                width: 100%;
            }

            &__info {
                width: 100%;
            }
        }
    }
}
</style>
