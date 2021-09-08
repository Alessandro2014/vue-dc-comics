<template>
    <!-- HEADER CON LINK DI NAVIGAZIONE -->
  <header class="container">
      <div class="row">
        <figure>
            <img src="@/assets/img/dc-logo.png" alt="logo">
        </figure>
        <ul v-for="(link, index) in links" :key="index">
            <li :class="{active: link.current}">
                <a :href="link.url">{{ link.text }}</a>
            </li>
        </ul>
    </div>
  </header>
</template>

<script>
export default {
    name: "Header",
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
        ],
        }
    }
}
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";

.row {
    height: 120px;
    figure {
        flex-grow: 1;
        img {
            max-width: 80px;
            height: auto;
        }
    } 
  }

ul {
    li {
    display: flex;
    &.active {
        border-bottom: 2px solid $blue-color;
    }   
}
}

a {
    text-transform: uppercase;
    color: $gray-color;
    font-weight: bold;
    padding: 10px;
    &:hover {
        color: $blue-color;
    }
}
</style>