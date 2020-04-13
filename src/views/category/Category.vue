<template>
  <div class="wrapper">
    <ul class="content">
      <button @click="btnClick">按钮</button>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
      <li>122</li>
    </ul>
  </div>
</template>

<script>
  import BScroll from 'better-scroll'

  export default {
    name: "Category",
    data() {
      return {
        scroll: null
      }
    },
    mounted() {
      this.scroll = new BScroll(document.querySelector('.wrapper'), {
        probeType: 3,
        pullUpLoad: true
      })
      this.scroll.on('scroll', (position) => {
        console.log(position)
      })
      this.scroll.on('pullingUp', () => {
      })
    },
    methods:{
      btnClick(){
        console.log('监听按钮事件')
      }
    }
  }
</script>

<style scoped>
  .wrapper {
    height: 150px;
    background-color: red;
  }
</style>
