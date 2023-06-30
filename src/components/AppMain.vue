<script>
import ComicCard from './ComicCard.vue';

export default {
    props: {
        cards: Array
    },
    components: { ComicCard }
}
</script>

<template>
    <main>
        <section class="jumbotron">
            <a href="#">Current Series</a>
        </section>

        <ComicCard :cards="cards" />

    </main>
</template>

<style lang="scss" scoped>
@use '../assets/scss/vars' as *;
@use '../assets/scss/mixins' as *;

main {
    background-color: $lightBlack;
}



.jumbotron {
    height: 400px;
    background-image: url(../assets/img/jumbotron.jpg);
    background-size: cover;
    background-position: center top;
    background-repeat: no-repeat;
    position: relative;


    a {
        background-color: $blue;
        position: absolute;
        bottom: -8%;
        left: 18%;
        z-index: 1;
        color: $white;
        font-weight: 600;
        font-size: 25px;
        padding: 15px 20px;
        display: block;
        text-transform: uppercase;
    }
}
</style>