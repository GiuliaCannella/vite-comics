<script>
export default {
    data() {
        return {
            links: [
                {
                    title: 'characters',
                    url: '#',
                },
                {
                    title: 'comics',
                    url: '#'
                },
                {
                    title: 'movies',
                    url: '#',
                },
                {
                    title: 'tv',
                    url: '#',
                },
                {
                    title: 'games',
                    url: '#',
                },
                {
                    title: 'collectibles',
                    url: '#',
                },
                {
                    title: 'videos',
                    url: '#',
                },
                {
                    title: 'fans',
                    url: '#',
                },
                {
                    title: 'news',
                    url: '#',
                },
                {
                    title: 'shop',
                    url: '#',
                }
            ],
            indexLink: 1
        }
    },
    methods: {
        changePage(index) {
            this.indexLink = index;
        }
    },
}
</script>

<template>
    <div class="container d-flex justify-content-center align-items-center">
        <div class="container-logo w-30">
            <img src="/img/dc-logo.png" alt="">
        </div>
        <div class="container-links w-70">
            <ul>
                <li v-for="(link, index) in links">
                    <a @click="changePage(index)" :href="link.url" :class="index === indexLink ? 'active' : ''" class="">
                        {{ link.title }}
                    </a>
                </li>
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
                a {
                    border-bottom: 2px solid transparent;
                    text-transform: uppercase;
                    font-size: 0.8em;
                    padding: 0.8em;
                    text-decoration: none;
                    color: black;


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
}
</style>