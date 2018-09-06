<template>

  <header>
    <nav class="header-nav">
      <img src="../assets/logo.svg" alt="" class="header-logo">
      <ul class="header-link">
        <router-link tag="li" id="academy-nav" to="#about" exact><a class="header-a">講座について</a></router-link>
        <router-link tag="li" id="teacher-nav" to="#lecturer" exact><a class="header-a">講師</a></router-link>
        <router-link tag="li" id="schedule-nav" to="#schedule" exact><a class="header-a">スケジュール</a></router-link>
        <router-link tag="li" id="apply-nav" to="/form" exact><a class="header-a">お申し込み</a></router-link>
        <li id="contact-nav"  exact><a class="header-a" href="mailto:academy@unknownbooks.co.jp">お問い合わせ</a></li>
        <li tag="li" id="company-nav" exact><a class="header-a" href="https://unknownbooks.co.jp/">アンノーンブックスについて</a></li>

      </ul>
    </nav>
  </header>

</template>

<script>
export default {
  watch: {
    '$route': function (n, o) {
      if (n.hash.match(/^#/)) {
        document.getElementById(n.hash.replace(/^#/, '')).scrollIntoView()
      }
      console.log('new, old', [n.hash, o.hash])
    }
  },
  mounted () {
    if (this.$route.hash.match(/^#/)) {
      document.getElementById(this.$route.hash.replace(/^#/, '')).scrollIntoView()
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

  .header{
    &-nav{
      display: flex;
    }
    &-logo{
      width: 80px;
      height: auto;
      flex: 0 0 80px;
      padding: 0 5%;

    }
    &-link{
      flex: 1 1 100px;
      list-style: none;
      display: flex;
      padding-top: 5%;
      flex-wrap: wrap;

    }
    &-a{
      color: black;
      text-decoration: none;
      font-size: 12px;
      padding: 0 15px;
      font-weight: bold;
    }
  }

</style>
