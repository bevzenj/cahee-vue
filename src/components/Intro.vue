<template>
  <section class="intro" id="intro">
    <div class="container">
        <div class="intro-discr">
            <h2 class="intro-discr__title">
                Fresh Life
            </h2>
            <p class="intro-discr__text">
                Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                Ut enim ad minim veniam, quis nostrud exercitation ullamco.
            </p>
            <button class="general-button__btn intro__btn">
                get free now
            </button>
        </div>
    </div>
</section>
</template>

<script>
export default {
  name: 'Intro',
};
</script>

<style lang="scss">
.intro {
    color: #262626;
    background: url('~@/assets/image/intro/background_header.png');
    background-position: center center;
    position: relative;
    top: -60px;
    height: 900px;

    .container {
        display: flex;
        align-items: center;
        height: 100%;
    }

    &-discr {
        width: 35%;
    }

    &-discr__title {
        font-family: 'ralewayheavy', sans-serif;
        font-weight: 900;
        font-size: 60px;
    }

    &-discr__text {
        font-family: 'ralewaylight', sans-serif;
        font-weight: 300;
        font-size: 17px;
        margin-bottom: 30px;
    }

    &__btn {
        background: #ff5f33;
        padding: 15px 25px;
    }
}
</style>
