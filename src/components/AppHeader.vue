<script>
export default {
    data() {
        return {
            links: [
                {
                    text: 'Characters',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Comics',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Movies',
                    url: '#',
                    current: false,
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Games',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Collectibles',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Videos',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Fans',
                    url: '#',
                    current: false,
                },
                {
                    text: 'News',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Shop',
                    url: '#',
                    current: false,
                },
            ]
        }
    }
}
</script>

<template>
    <header>
        <div class=" header-container container">
            <figure>
                <img src="../assets/img/dc-logo.png" alt="logo">
            </figure>
            <nav>
                <ul>
                    <li v-for="link in links" key="link.text">
                        <a :href="link.url" :class="{ active: link.current }">{{ link.text }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use '../assets/scss/vars' as *;
@use '../assets/scss/mixins' as *;


.header-container {
    height: 100%;
    @include flexbox(space-between, center);
}

header {
    height: 110px;
    background-color: $white;
}

img {
    width: 80px;
}

ul {
    display: flex;

    li {
        padding: 0 10px;

        a {
            color: $lightBlack;
            font-weight: 600;
            text-transform: uppercase;
            font-size: 14px;

            &:hover,
            &.active {
                color: $blue;
                border-bottom: 5px solid $blue;
                padding-bottom: 40px;
            }
        }
    }
}
</style>