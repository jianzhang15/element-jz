<template>
  <div>
    <el-checkbox-group v-model="checkboxGroup1" :min="1">
      <el-checkbox-button v-for="city in cities" :label="city" :key="city">{{
        city
      }}</el-checkbox-button>
    </el-checkbox-group>
  </div>
</template>

<script>
export default {
  data() {
    return {
      checkboxGroup1: ["上海"],
      checkedCities: [],
      cities: ["上海", "北京", "广州", "深圳"],
    };
  },
};
</script>
