<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<style lang="scss">
@font-face {
    font-family: 'pacificoregular';
    src: url('~@/assets/fonts/pacifico/pacifico-webfont.eot');
    src: url('~@/assets/fonts/pacifico/pacifico-webfont.woff2') format('woff2'),
         url('~@/assets/fonts/pacifico/pacifico-webfont.woff') format('woff');
    font-weight: 400;
    font-style: normal;
}

@font-face {
    font-family: 'ralewaybold';
    src: url('~@/assets/fonts/raleway/raleway-bold-webfont.eot');
    src: url('~@/assets/fonts/raleway/raleway-bold-webfont.woff2') format('woff2'),
         url('~@/assets/fonts/raleway/raleway-bold-webfont.woff') format('woff');
    font-weight: 700;
    font-style: normal;
}

@font-face {
    font-family: 'ralewayheavy';
    src: url('~@/assets/fonts/raleway/raleway-heavy-webfont.eot');
    src: url('~@/assets/fonts/raleway/raleway-heavy-webfont.woff2') format('woff2'),
         url('~@/assets/fonts/raleway/raleway-heavy-webfont.woff') format('woff');
    font-weight: 900;
    font-style: normal;
}

@font-face {
    font-family: 'ralewaylight';
    src: url('~@/assets/fonts/raleway/raleway-light-webfont.eot');
    src: url('~@/assets/fonts/raleway/raleway-light-webfont.woff2') format('woff2'),
         url('~@/assets/fonts/raleway/raleway-light-webfont.woff') format('woff');
    font-weight: 300;
    font-style: normal;
}
.container {
  max-width: 1320px;
  margin: 0 auto;
}
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
.general-button {
    display: flex;
    justify-content: center;

    &__btn {
        font-family: 'ralewaylight', sans-serif;
        font-weight: 300;
        font-size: 20px;
        color: #ffffff;
        text-transform: uppercase;
        border: none;
        box-shadow: 3px 4px 6px 0 rgba(0,0,0,0.73);

        &:hover {
            box-shadow: 7px 6px 0px 2px rgba(0,0,0,0.73);
            transition-duration: 0.5s;
        }
    }
}
.general-title {
    text-align: center;
    font-family: 'ralewaybold', sans-serif;
    font-weight: 700;
    font-size: 90px;
}

.general-subtitle {
    text-align: center;
    font-family: 'ralewaylight', sans-serif;
    font-weight: 300;
    font-size: 17px;
}
</style>
