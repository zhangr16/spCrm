<template>
  
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
  <el-tab-pane label="公司主页">
      <el-button type="primary" @click = 'fn1'>膳品宅送PC</el-button>
      <el-button type="primary" @click = 'fn2'>膳品宅送mobile</el-button>
  </el-tab-pane>
</el-tabs>

</template>

<script>
    import User from './components/User.vue'
    import Schedule from './components/Schedule.vue'
    import Attendance from './components/Attendance.vue'
    import Customer from './components/Customer.vue'



    export default {
      data() {
        return {
            
           
        };
    },
    methods: {
     fn1: function(){
      window.open("https://www.3pzs.com");  
  },
  fn2: function() {
    window.open('https://t-m.3pzs.com')
}
},
components: {
   User,
   Schedule,
   Attendance,
   Customer
}
}
</script>

<style>
	.user-manage{
		
	} 
 
</style>
