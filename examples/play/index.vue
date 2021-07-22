<template>
  <div>
      <el-checkbox-group v-model="checkboxGroup1">
      <el-checkbox-button v-for="city in cities" :label="city" :key="city">{{city}}</el-checkbox-button>
    </el-checkbox-group>
    <el-checkbox-group 
    v-model="checkedCities"
    :min="1"
    :max="2">
    <el-checkbox v-for="city in cities" :label="city" :key="city">{{city}}</el-checkbox>
  </el-checkbox-group>
  </div>
</template>

<script>
export default {
  data() {
    return {
      checkboxGroup1: ['上海'],
      checkedCities:[],
      cities:['上海', '北京', '广州', '深圳']
    };
  },
};
</script>
