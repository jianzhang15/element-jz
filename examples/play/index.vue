<template>
  <el-table
        ref="table"
        class="table-fixed"
        border
        :data="[]"
        row-key="sampleId"
      >
        <el-table-column
          type="selection"
          width="50"
          align="center"
          fixed="left"
          reserve-selection
        />
        <el-table-column :label="'test'" align="center"/>
        <template v-for="(column, index) in columns">
          <el-table-column :label="''+column" align="center" :key="index"/>
        </template>
      </el-table>
</template>

<script>
export default {
  data() {
    return {
      columns:[]
    };
  },
  mounted(){
    setTimeout(() => {
      this.columns=[1,2,3]
    }, 1000);
  }
};
</script>
