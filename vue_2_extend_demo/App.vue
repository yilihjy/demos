<template>
  <div>
      <h1>单文件组件继承验证demo</h1>
      <base-comp title="Base组件"></base-comp>
      <extend-a-comp title="ExtendsA组件"></extend-a-comp>
      <extend-b-comp title="ExtendsB组件"></extend-b-comp>
  </div>
</template>

<script>
import BaseComp from './Base.vue'
import ExtendAComp from './ExtendA.vue'
import ExtendBComp from './ExtendB.vue'

export default {
    name: 'App',
    components: {
        BaseComp,
        ExtendAComp,
        ExtendBComp
    }
}
</script>

<style>

</style>