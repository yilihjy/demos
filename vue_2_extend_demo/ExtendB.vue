<template>
  <div>
      <!-- 单文件组件的模板会整个替换 -->
      <h2>标题:{{title}}</h2>
      <p>{{count}} x 2 = {{doubleCount}}</p>
      <p class="text" @click="onClick">我被点击了{{count}}次</p>
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
.text {
    cursor: pointer;
}
</style>