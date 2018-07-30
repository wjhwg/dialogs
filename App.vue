<template>
  <div id="app">
    <div class="arrow_mask"></div>
    <div class="arrow-body" ref="arrow">
        <div class="arrow-body-header">
            萌店火拼节拼团规则
        </div>
        <div  class="arrow-body-text">
          <div class="text-mes">
              1、活动时间：2016年11月7日10点至2016年11月14日10点。其中，2016年11月10日22点至2016年11月14日10点为活动正式开抢时间，其余时间用户可抢先收藏活动商品，提前了解“11.11萌店火拼节”活动价。
          </div>
            <div class="text-mes">
              2、活动期间一个用户ID所获红包同一订单均不可叠加使用。红包不适用于秒杀团。红包具体使用规则可以进入萌店app“萌团长-卡券”查看，红包一经使用概不退回。
            </div>
            <div class="text-mes">
                3、红包活动仅面向萌店普通消费者，在获取和使用红包过程中，若出现违规行为（如作弊领取、恶意套取等），萌店有权取消批量刷取的抵用券使用权（含已使用的抵用券和未使用的抵用券）。
            </div>
            <div class="text-mes">
                4、萌店拥有法律范围内的活动解释权。
            </div>
            <div class="close">
                <img src="../src/assets/logo.png"  alt="picture"/>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
    export default {
     data () {
       return {

       }
     },
     mounted() {
      let sightHeight =  window.innerHeight || document.documentElement.clientHeight || document.body.clientHeight;
      let top = (sightHeight-350)/2;
      console.log(top)
       this.$refs.arrow.style.top = top +'px';
     }
    }
</script>

<style >
*{
  margin:0;
  padding: 0;
}
    .arrow_mask {
    /* display: none; */
    position: fixed;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    z-index: 1600;
    background: #333333;
    opacity: 0.8;
    width: 100%;
    height: 3000px;
}

.arrow-body{
    /* display: none; */
    width: 82%;
    height: 362px;
    position: absolute;
    z-index: 1601;
    /* top: 80px; */
    background: #ffffff;
    border-radius: 8px;
    margin-left: 9%;
}
.arrow-body-header{
    height: 46px;
    line-height: 46px;
    color: #FFFFFF;
    background: #ee0a3b;
    text-align: center;
    border-top-left-radius: 8px;
    border-top-right-radius: 8px;
    font-size: 16px;
}
.arrow-body-text{
    font-size: 11px;
    color: #333;
}
.text-mes{
    margin-top: 10px;
    width: 100%;
    padding-right: 20px;
    padding-left: 20px;
}
.close img{
    width: 40px;
    height: 40px;
    position: absolute;
    left: 50%;
    margin-left: -20px;
    bottom: -20px;
}
</style>
