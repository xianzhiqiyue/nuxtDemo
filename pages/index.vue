<template>
  <div class="container">
    <el-carousel class="banner-wrap" height="30vw">
      <el-carousel-item v-for="item in bannerList" :key="item.url">
        <div class="banner" :style="`background-image: url(${item.url});`" />
      </el-carousel-item>
    </el-carousel>
    <section>
      <p>大国重器 中国高端制造标杆</p>
      <p />
    </section>
  </div>
</template>

<script>
export default {
  data () {
    return {
      bannerList: [
        { url: 'https://www.xcmg.com/resources/web/img/ipart03.jpg' },
        { url: 'https://cos-www.sanygroup.com/2020/10/1f8d253fa4be46669b5d2e7d63007f36.png' },
        { url: 'https://cos-www.sanygroup.com/2020/10/38123f4be5b348d1bcacfd9352b5c77f.jpg' }

      ]
    }
  }
}
</script>

<style lang="scss">
.container{
  padding-top: calc(35vw + 60px);
}
.banner-wrap{
  position: fixed;
  top: 60px;
  width: 100vw;
  .banner{
    height: 35vw;
    background-size: cover;
  }
}
</style>
