<template>
  <!-- 组件结构 -->
  <div class="demo">
    <h2>姓名：{{stuName}}</h2>
    <h2>年龄：{{age}}</h2>
    <button @click="showName">点我提示姓名</button>
  </div>
</template>

<script>
  // 组件交互脚本
  const student = {
    name: 'Student',
    data(){
      return{
        stuName: 'dd',
        age: 12
      }
    },
    methods:{
      showName(){
        console.log(this.stuName)
      }
    }
  }
  export default student
</script>

<style>
/* 组件样式 */
.demo{
  background: orange
}
</style>