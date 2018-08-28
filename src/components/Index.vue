<template>

  <main>

    <div class="ct1" id="about">
      <img src="../assets/ct1.jpg" alt="Creatve writeing Academy " class="img-responsive center-block pc_display">
      <img src="../assets/ct1-m.jpg" alt="書店イベント一覧" class="img-responsive center-block sp_display">
    </div>

    <div class="ct2">
      <img src="../assets/ct2.jpg" alt="About Creatve writeing Academy " class="img-responsive center-block pc_display">
      <img src="../assets/ct2-m.jpg" alt="書店イベント一覧" class="img-responsive center-block sp_display">
      <router-link to="/form" exact><btn class="btn">お申し込みはこちら</btn></router-link>

    </div>

    <div class="ct3">
      <img src="../assets/ct3.jpg" alt="four features" class="img-responsive center-block pc_display">
      <img src="../assets/ct3-m.jpg" alt="書店イベント一覧" class="img-responsive center-block sp_display">
    </div>

    <div class="ct4">
      <img src="../assets/ct4.jpg" alt="four features" class="img-responsive center-block pc_display">
      <img src="../assets/ct4-m.jpg" alt="書店イベント一覧" class="img-responsive center-block sp_display">
    </div>

    <div class="ct5" id="lecturer">
      <img src="../assets/ct5.jpg" alt="four features" class="img-responsive center-block pc_display">
      <img src="../assets/ct5-m.jpg" alt="書店イベント一覧" class="img-responsive center-block sp_display">
    </div>

    <div class="ct5" id="">
      <img src="../assets/0.jpg" alt="four features" class="img-responsive center-block pc_display">
      <img src="../assets/0m.jpg" alt="書店イベント一覧" class="img-responsive center-block sp_display">
      <a href="https://form.run/@unknownbooks-cwa"><btn class="btn-2">お申し込みはこちら</btn></a>
    </div>

    <div class="ct6" id="schedule">
      <img src="../assets/ct6.jpg" alt="four features" class="img-responsive center-block pc_display">
      <img src="../assets/ct6-m.jpg" alt="書店イベント一覧" class="img-responsive center-block sp_display">
    </div>

    <div class="ct7">
      <img src="../assets/ct7.jpg" alt="four features" class="img-responsive center-block pc_display">
      <img src="../assets/ct7-m.jpg" alt="書店イベント一覧" class="img-responsive center-block sp_display">
    </div>

    <div class="ct8">
      <img src="../assets/ct8.jpg" alt="four features" class="img-responsive center-block pc_display">
      <img src="../assets/ct8-m.jpg" alt="書店イベント一覧" class="img-responsive center-block sp_display">
      <router-link to="/form" exact><btn class="btn-2">お申し込みはこちら</btn></router-link>

    </div>

    <div class="ct9">
      <img src="../assets/ct9.jpg" alt="four features" class="img-responsive center-block pc_display">
      <img src="../assets/ct9-m.jpg" alt="書店イベント一覧" class="img-responsive center-block sp_display">
    </div>

  </main>

</template>

<script>
export default {

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  $breakpoint-sm: 400px !default;
  $breakpoint-md: 768px !default;
  $breakpoint-lg: 1000px !default;
  $breakpoints: (
          'sm': 'screen and (max-width: 400px)',
          'md': 'screen and (max-width: 768px)',
          'lg': 'screen and (max-width: 1000px)',
          'xl': 'screen and (max-width: 1200px)',
  ) !default;
  @mixin mq($breakpoint: md) {
    @media #{map-get($breakpoints, $breakpoint)} {
      @content;
    }
  }
  h1, h2 {
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
  main {
    font-family: Georgia,游明朝,"Yu Mincho",YuMincho,"Hiragino Mincho ProN",HGS明朝E,メイリオ,Meiryo,serif;
  }
  .img-responsive{
    max-width: 100%;
    height: auto;
  }
  .center-block{
    display: block;
    margin-left: auto;
    margin-right: auto;
  }

  .btn{
    background: #E3357F;
    padding: 15px 130px;
    text-align: center;
    display: inline-block;
    color: white;
    text-decoration: none;
    margin-top: -10px;
    margin-bottom: 3%;
    &:hover{
      opacity: 0.8;
      transition: all .2s;
    }
    @include mq{
      padding: 15px 30px;
    }
  }
  .btn-2{
    background: #E3357F;
    padding: 15px 130px;
    text-align: center;
    display: inline-block;
    color: white;
    text-decoration: none;
    margin: -120px auto 0 auto;
    left: 30%;
    position: absolute;
    &:hover{
      opacity: 0.8;
      transition: all .2s;
    }
    @include mq{
      padding: 10px 30px;
      margin: -60px auto 0 auto;
    }
  }
  .ct3 {
    padding: 0 2%;
  }

  .ct4 {
    padding: 0 2%;
  }
  .ct5 {
    padding: 0 2%;
  }
  .ct6 {
    padding: 2%;
  }
  .ct7 {
    padding: 2%;
  }
  .ct8 {
    padding: 2%;
  }
  .ct9 {
    padding: 0 2% 0 2%;
  }

  @media only screen and (min-width: 768px) {
    /* PC、スマホ切り替え */
    .pc_display{
      display:block !important;
    }
    .sp_display{
      display:none !important;
    }
  }

  @media only screen and (max-width: 767px) {
    /* PC、スマホ切り替え */
    .pc_display{
      display:none !important;
    }
    .sp_display{
      display:block !important;
    }

    .lank{
      margin-bottom: 10%;
    }
    .lank .amazon{
      width: 95%;
      padding: 5% 0 9%;
    }
    .lank .btn{
      width: 95%;
      margin: 0 auto;
      position: static;
    }

    .cta01{
      margin-bottom: -10%;
    }
    .cta01 .btn{
      width: 34%;
      position: absolute;
      bottom: 41%;
      left: 0;
      right: 0;
      margin: auto;
    }

    .cta02 .btn{
      width: 34%;
      position: absolute;
      bottom: 8%;
      left: 0;
      right: 0;
      margin: auto;
    }

    .key .btn{
      width: 71%;
      margin: 0 auto;
      position: static;
    }

    .movie{
      width: 100%;
    }
    .movie iframe{
      height: 230px;
    }

    footer .logo{
      width: 28%;
      margin: 10% auto 5%;
    }

  }
</style>
