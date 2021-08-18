<template>
<footer class="footer">
    <div class="container">
        <div class="footer-copyright">
            &copy; 2015 Company. All right reserved
        </div>
        <div class="footer-logo">
            Cahee
        </div>
        <div class="footer-author">
            Made with
            <span class="footer-authot--red">love</span> by Auskteez
        </div>
    </div>
</footer>
</template>

<script>
export default {
  name: 'Footer',
};
</script>

<style lang="scss">
.footer {
    background: #262626;
    color: #b9b9b9;

    .container {
        display: flex;
        align-items: center;
        justify-content: space-between;
        height: 90px;
    }

    &-copyright {
        font-family: 'ralewaylight', sans-serif;
        font-weight: 300;
        font-size: 16px;
    }

    &-logo {
        font-family: 'pacificoregular', sans-serif;
        font-weight: 400;
        font-size: 25px;
    }

    &-author {
        font-family: 'ralewaylight', sans-serif;
        font-weight: 300;
        font-size: 15px;

        &--red {
            color: #ff2b58;
        }
    }
}

@media screen and (max-width: 768px) {
    .footer {
        &-copyright {
            width: 30%;
        }

        &-author {
            width: 30%;
        }
    }
}
</style>
