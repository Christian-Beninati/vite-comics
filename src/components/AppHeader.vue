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

<style scoped>
.header-container {
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

header {
    height: 110px;
    background-color: white;
}

img {
    width: 80px;
}

ul li a {
    color: black;
    font-weight: 600;
    text-transform: uppercase;
    font-size: 14px;
}

ul {
    display: flex;
}

ul li {
    padding: 0 10px;
}

ul li a:hover,
ul li a.active {
    color: #2982F9;
    border-bottom: 5px solid #2982F9;
    padding-bottom: 40px;
}
</style>