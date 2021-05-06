<template>
  <div class="header">
    <!-- <img src="" alt="" class="logo"> -->
    <div class="header-wrap">
      <section class="logo-wrap">
        <span>LOVELY</span>
      </section>

      <section class="menu">
        <span>关于我们</span>
        <span>官方商城</span>
        <span>解决方案</span>
        <span>新闻活动</span>
        <span>联系我们</span>
      </section>

      <section class="search">
        <i class="el-icon-search" />
      </section>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      activeIndex: '1'
    }
  },
  methods: {
    handleSelect (key, keyPath) {
      console.log(key, keyPath)
    }
  }
}
</script>

<style lang="scss" scoped>
.header{
  position: fixed;
  top: 0;
  width: 100vw;
  display: flex;
  justify-content: center;
  background-color: $mainColor;
  color: #fff;
  font-size: 18px;
  font-weight: bold;
}
.header-wrap{
  width: 500px;
  flex: 1 0 auto;
  max-width: 1320px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 60px;
  padding-left: 2vw;
  padding-right: 2vw;
}
.logo-wrap{
  span{
    font-size: 24px;
    font-weight: bold;
    font-family:'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    border-bottom: solid 3px #fff;
  }
}
.menu{
  :not(span:last-child) {
    margin-right: 20px;
  }
  span{
     cursor: pointer;
    &:hover{
      color: brown;
    }
  }
}
.search{
  i{
    cursor: pointer;
  }
}
</style>
