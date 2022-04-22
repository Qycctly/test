<template>
  <div>
    <h3>我是根组件</h3>
    <h3>scoped添加上给组件的标签新增一个自定义属性</h3>
    <Child1 />
  </div>
</template>

<script>
//引入子组件
//import Child from './components/Child.vue';
import Child1 from "./components/Child1.vue";

export default {
  //注册组件
  components: {
    Child1,
  },
};
</script>

<style scoped>
>>> h3 {
  color: red;
}
</style>