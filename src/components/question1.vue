<template>
  <div>
    <ul>
      <!-- 正确用法 -->
      <li v-for="(value, index) in testData" :key="index">
        <div v-if="Array.isArray(value)">
          <div v-for="(item, index) in value" :key="index">{{item}}</div>
        </div>
        <div v-else>{{value}}</div>

        <!-- 错误用法 -->
        <!-- <div v-if="Array.isArray(value)" v-for="(item, index) in value" :key="index">{{item}}</div>
        <div v-else>{{value}}</div>-->
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      testData: {
        name: "xiaomi",
        sex: "男",
        data: [100, 99, 98, 97]
      }
    };
  }
};
</script>

<style lang="scss" scoped>
</style>