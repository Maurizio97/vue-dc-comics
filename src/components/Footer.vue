<template>
  <footer>
    <!-- footer up -->
    <div id="background-img">
      <div class="centratura">
        <div class="nav-footer">
          <nav id="menu-items">
            <ul class="list-items">
            DC COMICS
              <li>
                voce 
              </li>
              <li>
                voce 
              </li>
              <li>
                voce 
              </li>
              <li>
                voce 
              </li>
              <li>
                voce 
              </li>
              <li>
                voce 
              </li>

            </ul>

            <ul class="list-items">
              DC
              <li>
                voce 
              </li><li>
                voce 
              </li><li>
                voce 
              </li><li>
                voce 
              </li><li>
                voce 
              </li><li>
                voce 
              </li><li>
                voce 
              </li>
            </ul>
                
            <ul class="list-items">
            SITE
              <li>
                voce 
              </li><li>
                voce 
              </li><li>
                voce 
              </li><li>
                voce 
              </li><li>
                voce 
              </li><li>
                voce 
              </li>
            </ul>
             
            <ul class="list-items">
            SHOP
              <li>
                voce 
              </li><li>
                voce 
              </li><li>
                voce 
              </li><li>
                voce 
              </li><li>
                voce 
              </li><li>
                voce 
              </li><li>
                voce 
              </li><li>
                voce 
              </li>
            </ul>

            <div id="logo-dc">
              <img src="../../public/assets/img/dc-logo-bg.png" alt="logo dc">

            </div>
            
          </nav>
        </div>
      </div>

    </div>
    
    <!-- footer down -->
    <div class="centratura">

    </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  footer {
    height: 61vh;
  }
  #background-img {
    background-image: url('../../public/assets/img/footer-bg.jpg');
    height: 80%;
    .nav-footer{
      /* display: flex; */
      .centratura {
        display: flex;
        justify-content: space-between;
        #menu-items {
          display: flex;
          flex-wrap: wrap;
          width: 50%;
          li {
            text-decoration: none;
          }
          .list-items {
            width: 50%;
          }
        }
        #logo-dc {
          height: 120%;
        }      
      }
    }
  }
</style>
