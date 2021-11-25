<template>
  <div class="item-comics">
      <div class="cont-img">
          <img :src="details.thumb" :alt="details.series">
      </div>
        <h3>
            {{details.series}}
        </h3>
  </div>
</template>

<script>
export default {
  name: 'ComicItems',
  props:{
      details:Object
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .item-comics {
        width: calc(100% / 6);
        padding: 30px /* 20px 50px 20px */;
    }
    .cont-img{
        height: 210px;
        overflow: hidden;
        img {
            width: 100%;
        }
    }
    h3 {
        color: white;
        margin-top: 20px;
    }
</style>
