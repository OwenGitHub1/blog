<template>
  <div>
      <MyNav></MyNav>
      <br>
      <br>
      <br>
      <br>
      <br>
      <el-row>
          <el-col :span="1">&nbsp;</el-col>
          <el-col :span="22">
              <el-carousel :interval="4000" type="card" height="300px">
                  <el-carousel-item><img src="../assets/test1.jpeg" class="cardPic"></el-carousel-item>
                  <el-carousel-item><img src="../assets/test2.jpeg" class="cardPic"></el-carousel-item>
                  <el-carousel-item><img src="../assets/test1.jpeg" class="cardPic"></el-carousel-item>
                  <el-carousel-item><img src="../assets/test2.jpeg" class="cardPic"></el-carousel-item>
                  <el-carousel-item><img src="../assets/test1.jpeg" class="cardPic"></el-carousel-item>
                  <el-carousel-item><img src="../assets/test2.jpeg" class="cardPic"></el-carousel-item>
              </el-carousel>

              <br>
              <div class="pageName">
                  <span class="title" style="float: left">最新文章</span>
                  <div style="float: right">
                      <el-button type="primary" round size="small">更多文章&nbsp;<i class="el-icon-d-arrow-right"></i></el-button>
                  </div>
              </div>
              <br>
              <div class="line"></div>
              <el-row>
                  <el-col :span="6" v-for = "item in 6" key="item">
                      <div class="item">
                          <img src="../assets/test1.jpeg" style="width: 200px">
                          <div>test name</div>
                      </div>
                  </el-col>
              </el-row>

              <br>
              <div class="pageName">
                  <span class="title" style="float: left">最新工具</span>
                  <div style="float: right">
                      <el-button type="primary" round size="small">更多工具&nbsp;<i class="el-icon-d-arrow-right"></i></el-button>
                  </div>
              </div>
              <br>
              <div class="line"></div>
              <el-row>
                  <el-col :span="6" v-for = "item in 6" key="item">
                      <div class="item">
                          <img src="../assets/test1.jpeg" style="width: 200px">
                          <div>test name</div>
                      </div>
                  </el-col>
              </el-row>
          </el-col>
          <el-col :span="1"></el-col>
      </el-row>
      <MyFooter></MyFooter>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import MyNav from '~/components/Nav.vue'
import MyFooter from '~/components/Footer.vue'

export default {
  components: {
    Logo,
    MyNav,
    MyFooter
  }
}
</script>

<style>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}

.cardPic{
    height: 300px;
}

.pageName{
    margin-bottom: 10px;
    margin-top: 10px;
}

.pageName .title{
    font-weight: bold;
    font-size: 20px
}

.line{
    border-bottom: 1px solid #e6e6e6;
    padding-top: 20px;
}

.item{
    text-align: center;
    padding-top: 10px;
    padding-bottom: 10px;
}
</style>
