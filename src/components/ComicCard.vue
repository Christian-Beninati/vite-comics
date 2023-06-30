<script>
export default {
    props: {
        cards: Array
    }
}
</script>

<template>
    <section class="container ">
        <div class="card-container">
            <div v-for="card in cards" :key="card.series" class="card">
                <figure>
                    <img :src="card.thumb" :alt="card.series">
                </figure>
                <h3>{{ card.series }}</h3>
            </div>
        </div>
        <div class="load-more-button">
            <a href="#">Load More</a>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../assets/scss/vars' as *;
@use '../assets/scss/mixins' as *;

.card-container {
    @include flexbox(start, stretch, row, wrap);
    padding: 60px 0;
    gap: 30px;
}

.card {
    flex-basis: calc(100% / 6 - 30px);
    cursor: pointer;

    h3 {
        color: $white;
        font-size: 13px;
        font-weight: 400;
        text-transform: uppercase;
        padding: 15px 0;
    }

    img {
        display: block;
        width: 100%;
        height: 200px;
        object-fit: cover;
        object-position: center top;
    }
}

.load-more-button {
    @include flexbox(center, center, );
    padding-bottom: 25px;
}

a {
    background-color: $blue;
    width: 200px;
    color: $white;
    font-weight: 600;
    font-size: 15px;
    padding: 10px 10px;
    display: block;
    text-transform: uppercase;
    text-align: center;
}
</style>