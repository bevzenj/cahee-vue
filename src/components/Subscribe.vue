<template>
<section class="subscribe">
    <div class="container">
        <div class="subscribe-discr">
            <h2 class="general-title subscribe-discr__title">
                Subscribe to us
            </h2>
            <p class="general-subtitle subscribe-discr__subtitle">
                Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                Inventore id laborum deserunt sequi saepe repellendus provident.
                Consequatur cupiditate aliquam accusantium sed.
            </p>
        </div>
        <div class="subscribe-email">
            <input class="subscribe-email__input"
            type="email" id="useremail"
            name="useremail"
            placeholder="Your email adress..">
            <label for="usermail">
                <button class="general-button__btn subscribe-email__btn">
                    subscribe
                </button>
            </label>
        </div>
    </div>
</section>
</template>

<script>
export default {
  name: 'Subscribe',
};
</script>

<style lang="scss">
.subscribe {
    background: url('~@/assets/image/subscribe/bg.png') no-repeat top;
    height: 500px;

    &-discr {
        margin-top: 140px;
        width: 50%;

        &__title {
            text-align: left;
            font-size: 40px;
            margin-bottom: 30px;
            text-transform: capitalize;
        }

        &__subtitle {
            text-align: left;
        }
    }

    &-email {
        display: flex;

        &__input {
            width: 550px;
            padding: 13px 15px;
            margin-right: 30px;
        }

        &__btn {
            background: #96b92c;
            padding: 10px 40px;
        }
    }
}

@media screen and (max-width: 768px) {
    .subscribe {

        &-discr {
            width: 100%;
        }

        &-email {
            flex-wrap: wrap;

            &__input {
                width: 100%;
            }

            &__btn {
                margin-top: 20px;
            }
        }
    }
}
</style>
