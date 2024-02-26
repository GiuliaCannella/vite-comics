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
        <div class="container-card bar d-flex">
            <div class="card" v-for="hero in heroes" :key="heroes.series">
                <img :src="heroes.thumb" :alt="heroes.series">
                <h3>{{ heroes.series }}</h3>

            </div>
        </div>
    </section>

    <MainIcons />
</template>

<style lang="scss" scope>
@use '../assets/scss/partials/utils' as *;

.bar {
    width: 100%;
    height: 900px;
    background-color: black;
    color: white;
}

.jumbotron-bg {

    height: 400px;
    background-size: cover;
    background-image: url('../../public/img/jumbotron.jpg');

}

.container-card {
    display: flex;
    flex-wrap: wrap;
}

.card {
    width: calc(100% / 6);
    padding: 20px;

    .h3 {
        font-size: 80em;
    }
}
</style>
