<template>
  <div class="User">	

   <el-table :data="msg[0]" style="width: 100%">

    <el-table-column prop="id" label="ID" sortable >

    </el-table-column>

    <el-table-column prop="name" label="姓名" >

    </el-table-column>

    <el-table-column prop="brandname" label="部门" >

    </el-table-column>

    <el-table-column prop="address" label="介绍" >

    </el-table-column>

  </el-table>

</div>
</template>

<script>
	
  export default {
    data() {

      return {
       msg:[]	          
     }
   },
   created: function(){
     this.$http.jsonp('http://apis.juhe.cn/oil/region?key=5983d539047e0a387b0d482e621e5b0a&format=2&city=%E5%8C%97%E4%BA%AC%E5%B8%82').then(function(res){
      this.msg.push(res.body.result.data);
      console.log(this.msg)    		
    })
   }
 }
</script>


<style scoped>

</style>
