<template>
  <main>
      <div class="container">
          <div class="row">
              <!-- STAMPA DINAMICA ICONE -->
              <figure v-for="(icon, index) in icons" :key="index">
                  <img :src="GetImageUrl(icon.image)" :alt="icon.text">
                  <figcaption>{{ icon.text }}</figcaption>
              </figure>
          </div>
      </div>
  </main>
</template>

<script>
export default {
name:"Main",
data() {
        return {
         icons: [
            {
                image: "buy-comics-digital-comics.png",
                text: "DIGITAL COMICS",
            },
            {
                image: "buy-comics-merchandise.png",
                text: "DC MERCHANDISE",
            },
            {
                image: "buy-comics-subscriptions.png",
                text: "SUBSCRIPTION",
            },
            {
                image: "buy-comics-shop-locator.png",
                text: "COMIC SHOP LOCATOR",
            },
            {
                image: "buy-dc-power-visa.svg",
                text: "DC POWER VISA",
            },
        ],
    }
},
computed: {},
methods: {
    GetImageUrl(fileName) {
        return require("@/assets/img/" + fileName);
    }
}
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";
main {
    height: 170px;
    background-color: $blue-color;
    position: relative;
    z-index: 1;
    .container {
        max-width: 1200px;
        .row {
            justify-content: space-between;
        }
    }
}

figure {
    display: flex;
    align-items: center;
    height: 170px;
    img {
        max-width: 50px;
        height: 50px;
    }
    figcaption {
    margin-left: 10px;
    color: white;
    }
}
</style>