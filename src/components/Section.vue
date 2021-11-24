<template>
  <div>
    <!-- colore di background -->
    <div id="background-sec-1">
      <div class="centratura">
        <!-- section 1 -->
        <section>
          <h2>
            Content Goes Here
          </h2>
        </section>
        <!-- /section 1 -->
      </div>
    </div>
    <!-- /colore di background -->

    <div id="background-sec-2">
      <div class="centratura">
        <!-- section 2 -->
        <section>
            <div v-for="item, i in navMain" :key="i">
              <img :src="item.image" :alt="image">
              <a href="#">{{ item.text }}</a>
            </div>
        </section>
        <!-- /section 2 -->

      </div>
    </div>

  </div>
</template>

<script>
export default {
  name: 'Main',
  data() {
    return {
      navMain: [
        {
          text: "DIGITAL COMICS",
          image: "../assets/img/buy-comics-digital-comics.png",
        },
          {
            text: "DC MERCHANDISE",
            image: "../assets/img/buy-comics-merchandise.png",
          },
        {
          text: "SUBSCRIPTION",
          image: "../assets/img/buy-comics-shop-locator.png",
        },
        {
          text: "COMIC SHOP LOCATOR",
          image: "../assets/img/buy-comics-subscriptions.png",
        },
        {
          text: "DC POWER VISA",
          image: "../assets/img/buy-comics-digital-comics.png",
        },
    ]}
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  #background-sec-1 {
    background-color: black;
  }

  section {
    height: 140px;
    h2 {
    color: white;
    vertical-align: middle;
    line-height: 140px;
  }
  }
  
</style>
