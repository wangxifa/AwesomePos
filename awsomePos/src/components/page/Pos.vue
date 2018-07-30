<template>
    <div class="pos">
        <el-row>
            <el-col :span='7' class="pos-order" id="order-list">
                <el-tabs>
                    <el-tab-pane label="点餐">
                        <el-table>
                            <el-table-column prop="goodsName" label="商品名称"></el-table-column>
                            <el-table-column prop="dount" label="数量"></el-table-column>
                            <el-table-column prop="price" label="金额"></el-table-column>
                            <el-table-column  label="操作" fixed="right">
                                <template slot-scope="scope">
                                    <el-button @click="handleClick(scope.row)" type="text" size="small">查看</el-button>
                                    <el-button type="text" size="small">编辑</el-button>
                                </template>
                            </el-table-column>
                        </el-table>
                    </el-tab-pane>
                    <el-tab-pane label="挂单">
                        挂单
                    </el-tab-pane>
                    <el-tab-pane label="外卖">
                        外卖
                    </el-tab-pane>
                </el-tabs>
                
            </el-col>
            <el-col :span='7'>
                我是产品栏
            </el-col>
        </el-row>
    </div>
</template>

<script>
export default {
  name: "pos",
  data(){
      return{
          
      }
  },
  mounted(){
      var clientHight = document.documentElement.clientHeight;
      console.log(clientHeight);
      
  }
      
};
</script>

<style>
.pos-order {
  background-color: #f9fafc;
  border-right: 1px solid #c0ccda;
}
</style>
