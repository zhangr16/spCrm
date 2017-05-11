<template>
  <div class="balance">
    <el-tabs type="border-card">
     <el-tab-pane label="员工管理">
      <user></user>
    </el-tab-pane>
    <el-tab-pane label="日程管理">
      <schedule></schedule>
    </el-tab-pane>
    <el-tab-pane label="考勤管理">
      <attendance></attendance>
    </el-tab-pane>
    <el-tab-pane label="客户管理">
      <customer></customer>
    </el-tab-pane>
    <el-tab-pane label="财务管理">
      <balance></balance> 
    </el-tab-pane>
    <el-tab-pane label="公司主页">
      <homepage></homepage>
    </el-tab-pane>
  </el-tabs>
</div>
</template>

<script>
  import User from './components/User.vue'
  import Schedule from './components/Schedule.vue'
  import Attendance from './components/Attendance.vue'
  import Customer from './components/Customer.vue'
  import Homepage from './components/HomePage.vue'
  import Balance from './components/Balance.vue'
  
  export default {

    data() {
      return {

      };
    },
    components: {
     User,
     Schedule,
     Attendance,
     Customer,
     Homepage,
     Balance
   },

 }
</script>

<style>


</style>
