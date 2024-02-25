<script>
import MainIcons from './subcomponents/MainIcons.vue';
export default {
    components: {
        MainIcons
    }
}

</script>

<template>
    <div class="bar d-flex  align-items-center">
        <div class="container">
            Content goes here
        </div>
    </div>
    <MainIcons />
</template>

<style lang="scss">
@use '../assets/scss/partials/utils' as *;

.bar {
    width: 100%;
    height: 100px;
    background-color: black;
    color: white;
}
</style>
