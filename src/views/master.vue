<template>
    <div class="master">
        <Nav></Nav>
        <!-- <div class="master_all"> -->
            <div class="master_left"></div>
            <div class="master_right">
                <el-row :gutter="20" style="margin-top: 20px;">
                    <el-col :span="6"><div class="grid-content bg-purple"></div></el-col>
                    <el-col :span="6"><div class="grid-content bg-purple"></div></el-col>
                    <el-col :span="6"><div class="grid-content bg-purple"></div></el-col>
                    <el-col :span="6"><div class="grid-content bg-purple"></div></el-col>
                  </el-row>
            </div>
        <!-- </div> -->
    </div>
</template>
<script>
    import Nav  from './nav.vue'
    export default{
        name: 'master',
        components: {
            Nav
        }
    }
</script>
<style>
    .master{
        display: flex;
    }
    /* .master_all{
        border: 2px solid black;
        
    } */
    .master_left{
        width: 160px;
        height: 800px;
        float: left;
        border: 8px solid greenyellow;
        z-index:-1;
        margin-left: 160px;
    }
    .master_right{
        width: 100%;
        height: 800px;
        float: left;
        border: 8px solid green;
        z-index:-1;
    } 
    /* .el-row {
    margin-bottom: 20px;
    &:last-child {
      margin-bottom: 0;
    }
  } */
  .el-col {
    border-radius: 4px;
  }
  .bg-purple-dark {
    background: #99a9bf;
  }
  .bg-purple {
    background: #d3dce6;
  }
  .bg-purple-light {
    background: #e5e9f2;
  }
  .grid-content {
    border-radius: 4px;
    min-height: 36px;
  }
  .row-bg {
    padding: 10px 0;
    background-color: #f9fafc;
  }

</style>