<template>
  <el-table :data="tableData">
    <el-table-column prop="date" label="日期" width="180"> </el-table-column>
    <el-table-column prop="name" label="姓名" width="180"> </el-table-column>
    <el-table-column label="操作" width="120">
      <template slot-scope="scope">
       <el-link
          :underline="false"
          type="text"
        >
          查看详情
        </el-link>
        <el-link
          class='ml2'
          :underline="false"
          type="primary"
        >
          刷新
        </el-link>
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
          name: "王小虎"
        },
      ],
    };
  },
  mounted() {},
};
</script>
