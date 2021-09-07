<template>
  <header class="container">
      <div class="row">
        <figure>
            <img src="@/assets/img/dc-logo.png" alt="logo">
        </figure>
        <nav>
            <ul v-for="(link, index) in links" :key="index">
                <li :class="{active: link.current}"><a :href="link.url">{{ link.text }}</a></li>
            </ul>
        </nav>
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
.row {
    height: 120px;
    justify-content: space-between;

  }

nav ul {
    display: flex;
    align-items: center;
  }

li {
    list-style: none;
}

figure img {
    max-width: 80px;
    height: auto;
}

a {
    text-transform: uppercase;
    color: #464646;
    font-weight: bold;
    padding: 10px;
}

a:hover
 {
    color: #0282F9;
}

li.active {
    border-bottom: 3px;
    background-color: #0282F9;
}
</style>