<script></script>

<template>
    <main>
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
    @include flexbox(null, center);

    h2 {
        color: $white;
    }
}
</style>