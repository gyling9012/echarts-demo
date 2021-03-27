<template>
  <div id="mapBox" class="centerItem">{{ $route.query.mapBoxEchart }}</div>
</template>

<script>
import * as echarts from 'echarts'

export default {
  data() {
    return { mapBoxEchart: null }
  },
  mounted() {
    this.mapBoxEchart = echarts.init(document.getElementById('mapBox'))
  },
  methods: {
    geoCoordMap() {
      this.mapBoxEchart = echarts.init(document.getElementById('mapBox'))
      this.mapBoxEchart.dispose()
      this.mapBoxEchart.setOption({
        city: {
          安徽省铜陵: [117.81154, 30.945515],
          长春: [125.8154, 44.2584],
          长沙: [113.0823, 28.2568],
          贵阳: [106.6992, 26.7682],
          杨凌: [109.1162, 34.2004],
          济南: [117.1582, 36.8701],
          海口: [110.3893, 19.8516],
          沈阳: [123.1238, 42.1216],
          武汉: [114.3896, 30.6628],
          红安: [114.23, 31.1],
          昆明: [102.9199, 25.4663],
          杭州: [119.5313, 29.8773],
          成都: [103.9526, 30.7617],
          拉萨: [91.1865, 30.1465],
          天津: [117.4219, 39.4189],
          合肥: [117.29, 32.0581],
          呼和浩特: [111.4124, 40.4901],
          哈尔滨: [127.9688, 45.368],
          北京: [116.4551, 40.2539],
          南京: [118.8062, 31.9208],
          南宁: [108.479, 23.1152],
          南昌: [116.0046, 28.6633],
          乌鲁木齐: [87.9236, 43.5883],
          上海: [121.4648, 31.2891],
          三亚: [109.5, 18.2]
        },
        data: [
          [{ name: '合肥' }, { name: '长春', value: 66 }],
          [{ name: '合肥' }, { name: '长沙', value: 66 }],
          [{ name: '合肥' }, { name: '贵阳', value: 66 }],
          [{ name: '合肥' }, { name: '杨凌', value: 66 }],
          [{ name: '合肥' }, { name: '深圳', value: 66 }],
          [{ name: '合肥' }, { name: '济南', value: 66 }],
          [{ name: '合肥' }, { name: '海口', value: 66 }],
          [{ name: '合肥' }, { name: '沈阳', value: 66 }],
          [{ name: '合肥' }, { name: '武汉', value: 66 }],
          [{ name: '合肥' }, { name: '昆明', value: 66 }],
          [{ name: '合肥' }, { name: '合肥', value: 118 }],
          [{ name: '合肥' }, { name: '杭州', value: 66 }],
          [{ name: '合肥' }, { name: '成都', value: 66 }],
          [{ name: '合肥' }, { name: '拉萨', value: 66 }],
          [{ name: '合肥' }, { name: '天津', value: 66 }],
          [{ name: '合肥' }, { name: '呼和浩特', value: 66 }],
          [{ name: '合肥' }, { name: '哈尔滨', value: 66 }],
          [{ name: '合肥' }, { name: '北京', value: 66 }],
          [{ name: '合肥' }, { name: '南宁', value: 66 }],
          [{ name: '合肥' }, { name: '南昌', value: 66 }],
          [{ name: '合肥' }, { name: '乌鲁木齐', value: 66 }],
          [{ name: '合肥' }, { name: '上海', value: 66 }]
        ]
      })
    }
  }
}
</script>

<style>
.centerItem {
  width: 856px;
  height: 640px;
  background-color: #003077;
  margin: 110px auto 0 auto;
}
</style>
