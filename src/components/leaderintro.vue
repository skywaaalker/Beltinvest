<template>
<div class="page-intro-part">
    <img :src="`${require(`../assets/img/leaders/photo_${leadername}@2x.png`)}`"/>
    <h3>{{title}}</h3>
    <h6>{{subtitle}}</h6>
  <!-- <div class="intro-part-2">
    <p class="p1">{{title}}</p>
    <p class="p2">{{subtitle}}</p>
    <p class="p3">{{moreinfo}}</p>
  </div> -->

</div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      default: 'Alex Yan'
    },
    subtitle: {
      type: String,
      default: 'Black Fish Group CEO'
    },
    leadername: {
      type: String,
      default: 'yan'
    },
    moreinfo: {
      type: String,
      dafault: '途牛旅游网(NASDAQ TOUR)联合创始人，2006年开始担任途牛旅游网COO，总裁 2005年至2006年间是育儿网[HK:08361]COO'
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
    width: 170px;
    height: 250px;
    margin-top: 30px;
    display: inline-block;
    img{
    width: 130px;
    height: 170px;
    }
    h3{
    font-size: 14px;
    color: #c99d55;
    font-weight: 400;
    margin: 7px 0px;
    }
    h6{
    font-size: 12px;
    color: #999;
    margin: 6px 0px;
    text-align: center;
    }
}

</style>
