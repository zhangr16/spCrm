<template>
    <div class="Homepage">
        <el-button type="primary" @click = 'fn1'>膳品宅送PC</el-button>
        <el-button type="primary" @click = 'fn2'>膳品宅送mobile</el-button>        
    </div>
</template>

<script>
    export default {

        data() {
            return{
                form: {},
                value3: null
            }
        },
        methods: {
           fn1: function(){
              window.open("https://www.3pzs.com");  
          },
          fn2: function() {
              window.open('https://t-m.3pzs.com')
          },
      }        
  }


</script>

<style>
</style>