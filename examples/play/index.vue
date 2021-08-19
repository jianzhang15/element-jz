<template>
  <el-table :data="tableData">
    <el-table-column prop="date" label="日期" width="180"> </el-table-column>
    <el-table-column prop="name" label="姓名" width="180"> </el-table-column>
    <el-table-column prop="address" label="地址" width="120"  show-overflow-tooltip>
      <template slot-scope="scope">
        <div
          class="pointer"
        >
          <div>
            <span>检材名称：</span>
            <span
              v-text="scope.row.address || '-'"
              class="primary-color"
            ></span>
          </div>
          <div class="font12">
            检材编号：{{ scope.row.address || "-" }}
          </div>
        </div>
      </template>
    </el-table-column>
  </el-table>
</template>

<script>
export default {
  data() {
    return {
      tableData: [
        {
          date: "2016-05-02",
          name: "王小虎",
          address: "上海市普陀区金沙江路 1518 弄",
        },
      ],
    };
  },
  mounted() {},
};
</script>
