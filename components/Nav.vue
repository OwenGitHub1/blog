<template>
  <div class="myheader">
      <el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect">
        <el-row>
            <el-col :span="4">
                <img src="../assets/logo.png" class="logo">
            </el-col>
            <el-col :span="16">
                <el-menu-item index="1" @click="$router.push('/')"><span class="tab">首页</span></el-menu-item>
                <el-menu-item index="2" @click="$router.push('/blog')"><span class="tab">博客</span></el-menu-item>
                <el-menu-item index="3" @click="$router.push('/tool')"><span class="tab">工具</span></el-menu-item>
                <el-menu-item index="4" @click="$router.push('/about')"><span class="tab">关于</span></el-menu-item>
            </el-col>
        </el-row>
      </el-menu>
  </div>
</template>

<script>
  export default {
    data () {
      return {
        activeIndex: '1'
      }
    },
    methods: {
      handleSelect (key, keyPath) {
        console.log(key, keyPath)
      }
    }
  }
</script>


<style solt-scope>
.logo{
    height: 50px;
    padding-top: 5px;
}

.tab{
    font-weight: bold;
}

.myheader{
    width: 100%;
    position: fixed;
    z-index: 1500;
}
</style>