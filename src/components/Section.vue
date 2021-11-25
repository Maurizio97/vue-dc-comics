<template>
  <div id="container-main">
    <div id="container-sec-1">
      <!-- jumbotron  -->
      <div id="jumbotron"></div>
      <!-- /jumbotron  -->
      <div id="plate">
        CURRENT SERIES
      </div>
      <!-- items comics -->
      <div id="container-comics-items">
          <div class="centratura">
            
          </div>
      </div>
      <!-- /items comics -->
    </div>

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
      comicsCop: [
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
          "price": "$19.99",
          "series": "Action Comics",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
          "price": "$3.99",
          "series": "American Vampire 1976",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
          "price": "$16.99",
          "series": "Aquaman",
          "type": "graphic novel"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
          "price": "$2.99",
          "series": "Batgirl",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          "price": "$3.99",
          "series": "Batman",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          "price": "$2.99",
          "series": "Batman Beyond",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
          "price": "$3.99",
          "series": "Batman/Superman",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
          "price": "$4.99",
          "series": "Batman/Superman Annual",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
          "price": "$5.99",
          "series": "Batman: The Joker War Zone",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
          "price": "$6.99",
          "series": "Batman: Three Jokers",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
          "price": "$4.99",
          "series": "Batman: White Knight Presents: Harley Quinn",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
          "price": "$16.99",
          "series": "Catwoman",
          "type": "graphic novel"
        }
      ],
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
  // sezione 1
  #container-sec-1{
    position: relative;
  }

  #jumbotron {
    height: 400px;
    background-image: url("../../public/assets/img/jumbotron.jpg");
  }

  #plate{
    background-color: #0282f9;
    line-height: 40px;
    vertical-align: middle;
    text-align: center;
    color: white;
    height: 40px;
    width: 200px;
    position: absolute;
    left: 270px;
    top:380px
  }

  #container-comics-items{
    background-color: black;
    // debug
    height: 400px;
  }
  // /sezione 1

  // sezione 2
  #background-sec-2 {
    background-color: #0282f9;
    height: 130px;
    display: flex;

    section {
      height: 100%;
      display: flex;
      width: 100%;
      justify-content: space-between;

      .item{
        display: flex;
        align-items: center;
        height: 100%;
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
  // /sezione 2
</style>
