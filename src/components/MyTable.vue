<template>
  <div>
    <el-table :data="tableData">
      <el-table-column prop="date" label="Date" width="140"> </el-table-column>
      <el-table-column prop="name" label="Name" width="120"> </el-table-column>
      <el-table-column prop="address" label="Address"> </el-table-column>
    </el-table>
  </div>
</template>

<script>
// 這裡可以載入其它文件 (例如:組件、JS檔、第三方套件、Json檔案、圖片...等)
// EX: import 組件名稱 from '組件路徑';

export default {
  // import載入的組件需要注入到物件中才能使用
  components: {},
  props: {},
  data() {
    // 這裡放資料
    const item = {
      date: "2016-05-02",
      name: "Tom",
      address: "No. 189, Grove St, Los Angeles",
    };
    return {
      tableData: Array(20).fill(item),
    };
  },
  // 計算屬性，類似於data的概念
  computed: {},
  // 監聽器，監聽資料有無變化
  watch: {},
  // 方法集合
  methods: {},
  // 生命週期 - 建立完成 (可以訪問當前this實例)
  created() {},
  // 生命週期 - 掛載完成 (可以訪問DOM元素)
  mounted() {},
  beforeCreate() {}, // 生命週期 - 建立前
  beforeMount() {}, // 生命週期 - 掛載前
  beforeUpdate() {}, // 生命週期 - 更新前
  updated() {}, // 生命週期 - 更新後
  beforeDestroy() {}, // 生命週期 - 銷毀前
  destroyed() {}, // 生命週期 - 已銷毀
  activated() {}, // 如果頁面有keep-alive緩衝功能，這個函數就會觸發
};
</script>

<style alng='scss' scoped>
/* @import url(); 載入共用的css類別 */
</style>