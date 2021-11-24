<template>
  <header>
    <!-- contenitore per la centratura -->
    <div class="centratura">
      <!-- logo -->
      <div id="logo">
        <img src="assets/img/dc-logo.png" alt="logo dc">
      </div>

      <!-- nav bar -->
      <nav>
        <ul>
          <li v-for="menu, i in navBar" :key="i">   
            <a :href="menu.href" :class="menu.focus? 'active': ''">{{menu.text}}</a>
          </li>
        </ul>
      </nav>
    </div>
    <!-- <font-awesome-icon icon="user-secret"></font-awesome-icon>  --> <!-- test per fontawesome -->
  </header>
</template>

<script>
export default {
  name: 'Header',
  data() {
    return {
      navBar:[
        {
          text: "CHARACTERS",
          focus: false,
          href: "#"
        },
        {
          text: "COMICS",
          focus: true,
          href: "#"
        },
        {
          text: "MOVIES",
          focus: false,
          href: "#"
        },
        {
          text: "TV",
          focus: false,
          href: "#"
        },
        {
          text: "GAMES",
          focus: false,
          href: "#"
        },
        {
          text: "COLLECTIBLES",
          focus: false,
          href: "#"
        },
        {
          text: "VIDEOS",
          focus: false,
          href: "#"
        },
        {
          text: "FANS",
          focus: false,
          href: "#"
        },
        {
          text: "NEWS",
          focus: false,
          href: "#"
        },
        {
          text: "SHOP",
          focus: false,
          href: "#"
        },
      ]}}
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  header {
    margin: 20px 0;
    li {
      display: inline-block;
      a {
        text-decoration: none;
        padding: 15px 20px;
        font-size: 15px;
        color: black;
        font-weight: bold;
        &.active {
          background-color: gray;
        }
      }
    }
  }
    

  .centratura {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
</style>
