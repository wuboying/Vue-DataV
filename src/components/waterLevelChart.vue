<template>
  <div id="water-level-chart">
    <div class="water-level-chart-title">计划资金累计完成情况</div>

    <div class="water-level-chart-details">
      累计完成<span>235,680</span>元
    </div>

    <div class="chart-container">
	  <dv-decoration-9 style="width:150px;height:150px;">66%</dv-decoration-9>
    </div>
  </div>
</template>

<script>
export default {
  name: 'WaterLevelChart',
  data () {
    return {
      config: {
        data: [45],
        shape: 'round',
        waveHeight: 25,
        waveNum: 2
      }
    }
  }
}
</script>

<style lang="scss">
#water-level-chart {
  width: 20%;
  box-sizing: border-box;
  margin-left: 20px;
  background-color: rgba(6, 30, 93, 0.5);
  border-top: 2px solid rgba(1, 153, 209, .5);
  display: flex;
  flex-direction: column;
  .water-level-chart-title {
    font-weight: bold;
    height: 50px;
    display: flex;
    align-items: center;
    font-size: 18px;
    justify-content: center;
  }
  .water-level-chart-details {
    height: 12%;
    display: flex;
    justify-content: center;
    font-size: 15px;
    align-items: flex-end;
    span {
      font-size: 27px;
      font-weight: bold;
      color: #58a1ff;
      margin: 0 5px;
      margin-bottom: -5px;
    }
  }
  .chart-container {
    flex: 1;
    display: flex;
    justify-content: center;
    align-items: center;
  }
}
</style>