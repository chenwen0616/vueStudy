<template>
  <!-- 组件结构 -->
  <div class="demo">
    <h2>学校名称：{{schoolName}}</h2>
    <h2>学校地址：{{address}}</h2>
    <button @click="showName">点我提示学校名</button>
  </div>
</template>

<script>
  // 组件交互脚本
  const school = {
    name: 'School',
    data(){
      return{
        schoolName: '白云区学校',
        address: '白云区'
      }
    },
    methods:{
      showName(){
        console.log(this.schoolName)
      }
    }
  }
  export default school
</script>

<style>
/* 组件样式 */
.demo{
  background: orange
}
</style>