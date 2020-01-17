<template>
<div class="flex-center-center page-title-highlight">
  <img src="../assets/img/icons/ic_title@2x.png"/>
  <h3>{{title}}</h3>
  <img src="../assets/img/icons/ic_title@2x.png"/>
</div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      default: ''
    }
  },
  data () {
    return {
    }
  }
}
</script>

<style lang="less" scoped>
.page-title-highlight{
    width: 200px;
    margin: 0px auto;
    height: 42px;
  img{
    width: 22px;
    height: 22px;
    float: left;
    margin-top: 8px;
    margin-left: 8px;
    margin-right: 8px;
  }
  h3{
    font-size: 26px;
    color: #333;
    font-weight: 400;
    margin: 0rem 10px;
    float: left;
  }
}
</style>
