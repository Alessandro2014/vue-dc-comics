<template>
  <main>
      <div class="container">
          <div class="row">
              <figure>
                  <img src="@/assets/img/buy-comics-digital-comics.png" alt="digital">
                  <figcaption>DIGITAL COMICS</figcaption>
              </figure>
              <figure>
                  <img src="@/assets/img/buy-comics-merchandise.png" alt="merchandise">
                  <figcaption>DC MERCHANDISE</figcaption>
              </figure>
              <figure>
                  <img src="@/assets/img/buy-comics-subscriptions.png" alt="subscription">
                  <figcaption>SUBSCRIPTION</figcaption>
              </figure>
              <figure>
                  <img src="@/assets/img/buy-comics-shop-locator.png" alt="shop">
                  <figcaption>COMIC SHOP LOCATOR</figcaption>
              </figure>
              <figure>
                  <img src="@/assets/img/buy-dc-power-visa.svg" alt="visa">
                  <figcaption>DC POWER VISA</figcaption>
              </figure>
          </div>
      </div>
  </main>
</template>

<script>
export default {
name:"Main"
}
</script>

<style scoped lang="scss">
main {
    height: 170px;
    background-color: #0282F9;
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
    font-size: 0.8rem;
    }
}



</style>