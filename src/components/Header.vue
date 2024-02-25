<script>
export default {
    data() {
        return {
            links: [
                'characters',
                'comics',
                'movies',
                'tv',
                'games',
                'collectibles',
                'videos',
                'fans',
                'news',
                'shop'
            ],
            indexLink: 1
        }
    },
}
</script>

<template>
    <div class="container d-flex justify-content-center align-items-center">
        <div class="container-logo w-30">
            <img src="../assets/img/dc-logo.png" alt="">
        </div>
        <div class="container-links w-70">
            <ul>
                <li v-for="(link, index) in links" :class="index === indexLink ? 'active' : ''" class="">{{ link }}</li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss">
@use '../assets/scss/partials/mixins' as *;
@use '../assets/scss/partials/utils' as *;

.container {
    padding: 0.8em 0;

    .container-logo {
        img {
            width: 50px
        }
    }


    .container-links {
        ul {
            @include flexbox();
            list-style: none;

            li {
                border-bottom: 2px solid transparent;
                text-transform: uppercase;
                font-size: 0.8em;
                padding: 0.8em;


                &:hover,
                &.active {
                    border-bottom: 2px solid #0379f1;
                    cursor: pointer;
                    color: #0379f1;
                }
            }

        }
    }
}
</style>