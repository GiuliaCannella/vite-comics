<script>
import MainIcons from './subcomponents/MainIcons.vue';
export default {
    components: {
        MainIcons
    },
    props: {
        heroes: Array
    }
}

</script>

<template>
    <div class="jumbotron-bg d-flex flex-column  ">

    </div>
    <section id="heroes">
        <div class="container-card">
            <div class="card" v-for="hero in heroes" :key="hero.series">
                <img :src="hero.thumb" :alt="hero.series">
                <h3>{{ hero.series }}</h3>

            </div>
        </div>
    </section>

    <MainIcons />
</template>

<style lang="scss" scope>
@use '../assets/scss/partials/utils' as *;

.jumbotron-bg {

    height: 400px;
    background-size: cover;
    background-image: url('../../public/img/jumbotron.jpg');

}

.container-card {
    display: flex;
    flex-wrap: wrap;
    width: 100%;
    background-color: black;
    color: white;
    padding: 2em;

    .card {
        width: calc(100% / 6);
        padding: 20px;

        h3 {
            font-size: 0.8em;
            text-align: center;
            text-transform: uppercase;
        }

        img {
            width: 100%;
        }
    }
}
</style>
