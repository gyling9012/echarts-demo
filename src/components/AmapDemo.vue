<template>
  <div id="container"></div>
</template>
<script>
export default {
  data() {
    return {}
  },
  mounted() {
    this.loadAmap()
  },
  methods: {
    loadAmap() {
      var map = new AMap.Map('container', {
        center: [116.397428, 39.90923],
        // 卫星影像地图
        layers: [new AMap.TileLayer.Satellite()],
        //高德默认标准矢量图层
        //layers: [new AMap.TileLayer()],
        zoom: 13
      })
    }
  }
}
</script>
<style lang="less" scoped>
#container {
  width: 90%;
  height: 90%;
}
</style>
