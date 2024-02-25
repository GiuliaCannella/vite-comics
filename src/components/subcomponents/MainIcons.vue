<script>

export default {
    data() {
        return {
            icons: [
                {
                    url: 'comics-digital-comics.png',
                    text: 'digital comics'
                },
                {
                    url: 'comics-merchandise.png',
                    text: 'dc merchandise'
                },
                {
                    url: 'comics-subscriptions.png',
                    text: 'subscription'
                },
                {
                    url: 'comics-shop-locator.png',
                    text: 'comic shop locator'
                },
                {
                    url: 'dc-power-visa.svg',
                    text: 'dc power visa'
                },

            ]
        }
    },
}

</script>

<template>
    <div class="bg-blue">
        <div class="container d-flex align-items-center">
            <div class="icon align-items-center d-flex" v-for="icon in icons">
                <img :src="`img/buy-${icon.url}`" alt="">
                <p>{{ icon.text }}</p>
            </div>
        </div>
    </div>
</template>

<style lang="scss">
.bg-blue {
    background-color: #0379f1;
    width: 100%;
    z-index: 2;

    .container {
        padding: 1em 2em;

        .icon {
            width: calc(100% / 5);

            img {
                width: 30px;

            }

            p {
                color: white;
                text-transform: uppercase;
                font-size: 0.5em;
                margin-left: 1em;
            }
        }
    }
}
</style>
