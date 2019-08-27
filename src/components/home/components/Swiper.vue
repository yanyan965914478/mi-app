<template>
  <div>
    <mt-swipe :auto="3000" :continuous="true">
      <mt-swipe-item v-for="(item,index) in swiperArr" :key="index">
        <img :src="item.img" alt />
      </mt-swipe-item>
    </mt-swipe>
  </div>
</template>
<script>
export default {
  data () {
    return {
      swiperArr: [
        {
          id: 1,
          img:
            'http://cdn.cnbj1.fds.api.mi-img.com/mi-mall/939a2f677670d5c852b07ce574a78cae.jpg?thumb=1&w=720&h=360'
        },
        {
          id: 2,
          img:
            'http://cdn.cnbj1.fds.api.mi-img.com/mi-mall/5d40feacc4d4fc31b3e6e65aa9891ea5.jpg?thumb=1&w=720&h=360'
        },
        {
          id: 3,
          img:
            'http://cdn.cnbj1.fds.api.mi-img.com/mi-mall/63e0e2bf0e7cae90dd848823852a7247.jpg?thumb=1&w=720&h=360'
        }
      ]
    }
  }
}
</script>
<style scoped>
div {
  width: 100%;
  height: 320px;
  background: pink;
}
div img {
  width: 100%;
  height: 320px;
}
</style>
