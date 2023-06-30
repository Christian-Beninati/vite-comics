<script>
</script>

<template>
    <main>
        <section class="jumbotron">
            <a href="#">CURRENT SERIES</a>
        </section>
        <section class="container comic-card">
            <h2> -- Content goes here -- </h2>
        </section>
    </main>
</template>

<style lang="scss" scoped>
@use '../assets/scss/vars' as *;
@use '../assets/scss/mixins' as *;

main {
    background-color: $black
}

.comic-card {
    height: 110px;
    @include flexbox(start, center);

    h2 {
        color: $white;
    }

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
    }
}
</style>