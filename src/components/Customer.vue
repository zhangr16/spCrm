<template>
	<div class="customer">
		<el-tabs>
            <el-tab-pane label="客户" name="first">
                <el-table :data="tableData2" style="width: 100%" :row-class-name="tableRowClassName">
                    <el-table-column prop="date" label="日期" sortable width="180"></el-table-column>
                    <el-table-column prop="name" label="姓名" width="180"></el-table-column>
                    <el-table-column prop="address" label="地址"></el-table-column>
                    <el-table-column prop='value3' label="评分" sortable></el-table-column>
                </el-table>
            </el-tab-pane>
            <el-tab-pane label="联系人" name="second">
            <el-table
             :data="tableData2"
             style="width: 100%"
             :row-class-name="tableRowClassName">
             <el-table-column
             prop="date"
             label="日期"
             width="180">
            </el-table-column>
            <el-table-column
            prop="name"
            label="姓名"
            width="180">
            </el-table-column>
            <el-table-column
            prop="address"
            label="地址">
            </el-table-column>
            </el-table>
            </el-tab-pane>
            </el-tabs>
</div>
</template>

<script>
  export default {
    methods: {
      tableRowClassName(row, index) {
        if (index === 1) {
          return 'info-row';
      } else if (index === 3) {
          return 'positive-row';
      }
      return '';
  }
},
data() {
  return {
    

    tableData2: [{
      date: '2016-05-02',
      name: '王1虎',
      address: '上海市普陀区金沙江路 1518 弄',
      value3: 1,
      valuer:null
  }, {
      date: '2016-05-04',
      name: '王2虎',
      address: '上海市普陀区金沙江路 1518 弄',
      value3: 2,
      valuer:null
  }, {
      date: '2016-05-01',
      name: '王3虎',
      address: '上海市普陀区金沙江路 1518 弄',
      value3: 3,
      valuer:null
  }, {
      date: '2016-05-03',
      name: '王4虎',
      address: '上海市普陀区金沙江路 1518 弄',
      value3: 4,
      valuer:null
  }]
}
}
}
</script>

<style>
  .el-table .info-row {
    background: #c9e5f5;
}

.el-table .positive-row {
    background: #e2f0e4;
}
</style>