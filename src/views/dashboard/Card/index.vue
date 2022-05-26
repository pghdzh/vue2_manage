<template>
  <div>
    <el-row :gutter="10">
      <el-col :span="6">
        <el-card>
          <Detail title="总销售额" count="￥ 126560">
            <template slot="charts">
              <span>
                周同比 &nbsp; &nbsp;56.7%
                <i class="el-icon-caret-top" style="color:red;"></i>
              </span>
              <span>
                日同比 &nbsp; &nbsp;19.96%
                <i class="el-icon-caret-bottom" style="color:green"></i>
              </span>
            </template>
            <template slot="footer">
              <span>日销售额 ￥ 12423</span>
            </template>
          </Detail>
        </el-card>
      </el-col>
      <el-col :span="6">
        <el-card>
          <Detail title="访问量" count="88460">
            <template slot="charts">
              <lineChart/>
            </template>
             <template slot="footer">
              <span>日访问量 1234</span>
            </template>
          </Detail>
        </el-card>
      </el-col>
      <el-col :span="6">
        <el-card>
          <Detail title="支付笔数" count="88460">
            <template slot="charts">
              <barCharts/>
            </template>
             <template slot="footer">
              <span>转换率64%</span>
            </template>
          </Detail>
        </el-card>
      </el-col>
      <el-col :span="6">
        <el-card>
          <Detail title="运营活动效果" count="78%">
            <template slot="charts">
              <programChart>
                
              </programChart>
            </template>
             <template slot="footer">
               <span>
                周同比 &nbsp; &nbsp;56.7%
                <i class="el-icon-caret-top" style="color:red;"></i>
              </span>
              <span>
                日同比 &nbsp; &nbsp;19.96%
                <i class="el-icon-caret-bottom" style="color:green"></i>
              </span>
            </template>
          </Detail>
        </el-card>
      </el-col>
    </el-row>
  </div>
</template>

<script>
import Detail from "./Detail";
import lineChart from "./lineChart"
import barCharts from "./barChart"
import programChart from './programChart'
export default {
  name: "",
  components: {
    Detail,
    lineChart,
    barCharts,
    programChart
  },
};
</script>

<style>
</style>