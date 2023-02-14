<template>
  <div>
    <div class="title">周末去哪儿</div>
    <ul>
      <li
        class="item border-bottom"
        v-for="item of recommendList"
        :key="item.id"
      >
        <div class="item-img-wrapper">
          <img class="item-img" :src="item.imgUrl" />
        </div>
        <div class="item-info">
          <p class="item-title">{{ item.title }}</p>
          <p class="item-desc">{{ item.desc }}</p>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "HomeRecommend",
  data() {
    return {
      recommendList: [
        {
          id: "0001",
          imgUrl:
            "https://imgs.qunarzz.com/sight/p0/2206/9a/9a0455e3fe18bec4a3.water.jpg_200x200_44a011ee.jpg",
          title: "木兰草原",
          desc:
            "这里区域开阔，建筑很有蒙古特色；春夏之交，格桑花开的时候景色尤其漂亮。草原上有羊驼、矮马等动物，还可以骑马、射箭、观赏草原特色的歌舞表演和马术表演等。"
        },
        {
          id: "0002",
          imgUrl:
            "https://imgs.qunarzz.com/sight/p0/1805/af/af648beb7239c330a3.img.png_200x200_05da91a0.png",
          title: "武汉花博汇",
          desc:
            "花博汇集花卉旅游观光、创意农业体验、田园养生度假、亲水休闲游乐、美丽乡村体验、花卉贸易展销等功能于一体，满足人们回归自然、乡野度假的“慢生活”需求。"
        },
        {
          id: "0003",
          imgUrl:
            "https://imgs.qunarzz.com/sight/p0/2107/f7/f7ed8fdecce9d00fa3.img.jpg_200x200_4f3e0b09.jpg",
          title: "海昌极地海洋公园",
          desc: "在这里你将跨越南北极，看到来自极寒之地的各种珍稀的极地动物们！"
        },
        {
          id: "0004",
          imgUrl:
            "https://imgs.qunarzz.com/sight/p0/2107/fd/fd37ada9c1ea8273a3.water.jpg_200x200_d3e08ff9.jpg",
          title: "金龙水寨旅游景区",
          desc:
            "全国有名的莲花水乡。在距今2300年前的战国时代,在古汉阳蔡甸地区发生了伯牙和钟子期“高山流水识知音”的传奇故事,知音文化可以说是蔡甸地区的元典文化。"
        }
      ]
    };
  }
};
</script>

<style lang="stylus" scoped>
@import '~styles/mixins.styl'
.title
  line-height: .8rem
  background: #eee
  text-indent: .2rem
.item-img-wrapper
  overflow: hidden
  height: 0
  padding-bottom: 33.9%
  .item-img
    width: 100%
    height: 5rem
.item-info
  padding: .1rem
  .item-title
    line-height: .54rem
    font-size: .32rem
    ellipsis()
  .item-desc
    line-height: .4rem
    color: #ccc
    ellipsis()
</style>
