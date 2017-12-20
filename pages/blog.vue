<template>
    <div>
        <MyNav></MyNav>
        <div class="containerBody">
            <el-row>
                <el-col :span="1">&nbsp;</el-col>
                <el-col :span="16">
                    <div style="padding-top: 10px;padding-bottom: 10px">
                        <h3>最新文章</h3>
                    </div>
                    <div class="box">
                       <el-row>
                           <el-col :span="7">
                               <img src="../assets/test1.jpeg" class="img">
                           </el-col>
                           <el-col :span="17">
                               <div class="desItem">
                                   <a>
                                       <h3>Google推出Tacotron 2：结合WaveNet，深度神经网络 TTS 媲美专业级别</h3>
                                   </a>
                               </div>
                               <div class="des">
                                   <span>
                                       10月Deepmind宣布对WaveNet升级后，Google Brain近日宣布推出 Tacotron 2，两个团队的暗中较劲仍在继续。
                                   </span>
                               </div>
                           </el-col>
                       </el-row>

                    </div>
                </el-col>
                <el-col :span="5"></el-col>
                <el-col :span="1"></el-col>
            </el-row>
        </div>
        <MyFooter></MyFooter>
    </div>
</template>

<script>
	import MyNav from '~/components/Nav.vue'
	import MyFooter from '~/components/Footer.vue'

    export default {
	    components: {
          MyNav,
          MyFooter
	    }
    }
</script>

<style slot-scoped>
    .containerBody{
        padding-top: 60px;
    }
    .box{
        position: relative;
        left:0;
        top: 0;
        width: 100%;
        height: 176px;
        padding-bottom: 25px;
        padding-top: 25px;
        overflow: hidden;
        border-bottom:1px solid #E6E6E6;
    }

    .img{
        width: 240px;
        height: 145px;
        vertical-align: top;
        float: left;
        position: relative;
    }

    .word{
        padding-left: 22px;
        overflow: hidden;
    }

    .desItem{
        text-align: left;
        color: #5e6b73;
        line-height: 22px;
        padding: 15px 0;
    }

    .des{
        text-align: left;
        color: #5e6b73;
        font-size: 14px;
    }

    .img{
        width: 240px;
        height: 145px;
        vertical-align: top;
        padding: 10px;
    }
</style>