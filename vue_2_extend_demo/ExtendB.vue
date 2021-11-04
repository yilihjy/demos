<template>
  <div>
      <!-- 单文件组件的模板会整个替换 -->
      <h2>标题:{{title}}</h2>
      <p @click="onClick">我被点击次数:{{count}} x 2 = {{doubleCount}}</p>
  </div>
</template>

<script>
import BaseComp from './Base.vue';
export default {
    name: 'ExtendB',
    extends: BaseComp,
}
</script>


<style scoped>
p {
    cursor: pointer;
}
</style>