<template>
  <div class="status-bar">
    <el-row>
      <el-col :span="6">
        <el-button @click="btnClick">btn</el-button>
      </el-col>
    </el-row>
  </div>
</template>
<script>
export default {
  name: 'status-bar',
  data() {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
