<script>
</script>

<template>
    <main>
        <section class="jumbotron"></section>
        <section class="container">
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

section {
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
}
</style>