<template>
<div class="page-intro-part">
  <img :src="`${require(`../assets/img/icons/ic_${iconname}@2x.png`)}`"/>
  <br>
  <h3>{{title}}</h3>
  <h6>{{subtitle}}</h6>
</div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      default: '优质资产'
    },
    subtitle: {
      type: String,
      default: '精选优质借款人，小额分散，风险可控'
    },
    iconname: {
      type: String,
      default: 'zichan'
    }
  },
  data () {
    return {
    }
  }
}
</script>

<style lang="less" scoped>
.page-intro-part{
    width: 250px;
    height: 100px;
    margin-top: 49px;
    display: inline-block;
  img{
    width: 42px;
    height: 42px;
  }
  h3{
    font-size: 13px;
    color: #666;
    font-weight: 400;
    margin: 7px 0px;
  }
  h6{
    font-size: 11px;
    color: #999;
    margin: 6px 0px;
    text-align: center;
  }
}
</style>
