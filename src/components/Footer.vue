<template>
  <footer>
    <!-- footer up -->
    <div id="background-img">
      <div class="centratura">
        <!-- contenitore logo e menu del footer -->
        <div class="nav-footer">

          <!-- menu footer -->
          <div id="menu-items" class="clearfix">
            <ul class="list-items" v-for="item, i in menuFooter" :key="i">
              {{item.title}}
              <li v-for="subItem, i in item.subMenu" :key="i">
                <a href="">{{subItem.section}}</a>
              </li>
            </ul>
          </div>
          <!-- /menu footer -->

          <!-- logo footer -->
          <div id="logo-dc">
            <!-- <img src="../../public/assets/img/dc-logo-bg.png" alt="logo dc" /> -->
          </div>
          <!-- /logo footer -->

        </div>
      </div>
    </div>

    <!-- footer down -->
    <section id="footer-down">
      <div class="centratura">
        Qui ci sarà il footer ma sono rimasto indietro e lo farò successivamente 
      </div>
    </section>
  </footer>
</template>

<script>
export default {
  name: "Footer",
  data() {
    return {
      menuFooter: [
        {
          title: "SITE",
          subMenu: [
            {
              section: "Characters"
            },
            {
              section: "Characters"
            },
            {
              section: "Characters"
            },
            {
              section: "Characters"
            },
            {
              section: "Characters"
            },
            {
              section: "Characters"
            },
            
          ]
        },
        {
          title: "DC",
          subMenu: [
            {
              section: "Characters"
            },
            {
              section: "Characters"
            },
            {
              section: "Characters"
            },
            {
              section: "Characters"
            },
            {
              section: "Characters"
            },
            {
              section: "Characters"
            },
            {
              section: "Characters"
            },
            {
              section: "Characters"
            },
            {
              section: "Characters"
            },
            {
              section: "Characters"
            },
          ]
        },
        
        {
          title: "DC COMICS",
          subMenu: [
            {
              section: "Characters"
            },
            {
              section: "Characters"
            },
            {
              section: "Characters"
            },
            {
              section: "Characters"
            },
            {
              section: "Characters"
            },
            {
              section: "Characters"
            },
            {
              section: "Characters"
            },
          ]
        },
        {
          title: "SHOP",
          subMenu: [
            {
              section: "Characters"
            },
            {
              section: "Characters"
            },
          ]
        },
      ]
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

footer {
  height: 600px;
}

// footer up
#background-img {
  background-image: url("../assets/img/footer-bg.jpg");
  height: 80%;

  .centratura {
      height: 100%;

    .nav-footer {
      display: flex;
      height: 100%;

      #menu-items {
        padding: 40px 20px;
        height: 100%;
        width: 50%;

        .list-items {
          width: calc( 100% / 3);
          float: right;
          color: white;
          margin: 20px 0;
          
          li  {
            margin-top:5px ;
            list-style: none;
            line-height: 1.6;

            a {
              text-decoration: none;
              color: grey;
              font-size: 12px;
            }
          }
        }
      }
      
      #logo-dc {
        height: 100%;
        width: 50%;
        display: flex;
        justify-content: flex-end;
      
        img {
          height: 100%;
          width: 75%;
          object-fit: none;
          
        }
      }
    }
  }
}
// /footer up


// footer down
#footer-down {
  height: 20%;
  // debug
  display: flex;
  align-items: center;
  background-color: red;
  font-size: 20px;
  font-weight: bold;
}
// /footer down
</style>
