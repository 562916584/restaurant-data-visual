<template>
  <div>
    词云 
  </div>
</template>

<script>
import axios from 'axios';//用于发请求
export default {
  props: ['curRestId'],
  watch: {//  仅测试使用
    curRestId: {
      deep: true,
      handler: function () {
        console.log('词云',  this.curRestId)
      }
    }
  }
}
</script>

<style lang="sass" scoped>

div
  font-size: 30px;
  padding: 30px;
  width: 100%;
  height: 100%;
  box-sizing: border-box;
  text-align: center;
</style>
