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

    <!-- colore di background -->
    <div id="background-sec-2">
      <div class="centratura">
        <!-- section 2 -->
        <section>
            <div class="item" v-for="item, i in navMain" :key="i">
              <img :src="item.image" :alt="image">
              <a href="#">{{ item.text }}</a>
            </div>
        </section>
        <!-- /section 2 -->
      </div>
    </div>
    <!-- /colore di background -->

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
          image: "assets/img/buy-comics-digital-comics.png",
        },
        {
          text: "DC MERCHANDISE",
          image: "assets/img/buy-comics-merchandise.png",
        },
        {
          text: "SUBSCRIPTION",
          image: "assets/img/buy-comics-shop-locator.png",
        },
        {
          text: "COMIC SHOP LOCATOR",
          image: "assets/img/buy-comics-subscriptions.png",
        },
        {
          text: "DC POWER VISA",
          image: "assets/img/buy-dc-power-visa.svg",
        },
    ]}
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  #background-sec-1 {
    background-color: black;

    section {
      height: 140px;
      h2 {
        color: white;
        vertical-align: middle;
        line-height: 140px;
      }
    }
  }

  #background-sec-2 {
    background-color: #0282f9;

    section {
      height: 155px;
      display: flex;
      width: 100%;
      justify-content: space-between;

      .item{
        display: flex;
        align-items: center;
        img { 
          height: 50px;
          margin: 10px;
        }
        &:last-child img{
          height: 35px;
        }
        a {
          color: white;
          text-decoration: none;
          font-weight: bold;
          font-size: 14px;
        }
      }
    }
  }
  
</style>
