<script>
import BaseComp from './Base.vue';
export default {
    name: 'ExtendA',
    extends: BaseComp,
    methods: {
        /**
         * 覆盖base的点击处理事件
         */
        onClick () {
            this.count --;
        }
    }
}
</script>

<style scoped>
/** 注意，继承组件覆盖了整个样式表, 所以现在组件没有边框 */
p {
    color: red;
}
</style>