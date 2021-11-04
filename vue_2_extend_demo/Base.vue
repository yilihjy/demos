<template>
  <div>
      <h2 @click="onClick">标题:{{title}}</h2>
      <p>标题被点击次数:{{count}} x 2 = {{doubleCount}}</p>
  </div>
</template>

<script>
export default {
    name: 'Base',
    props: ['title'],
    data () {
        return {
            count: 0
        }
    },
    computed: {
        doubleCount () {
            return this.count * 2
        }
    },
    methods: {
        onClick () {
            this.count ++;
        }
    }
}
</script>

<style scoped>
h2 {
    cursor: pointer;
}
p {
    color: rebeccapurple;
}
div {
    border: #CCC solid 1px;
}
</style>