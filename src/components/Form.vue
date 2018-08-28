<template>

  <section>
    <!-- Begin MailChimp Signup Form -->
    <link href="//cdn-images.mailchimp.com/embedcode/classic-10_7.css" rel="stylesheet" type="text/css">
    <div id="mc_embed_signup">
      <form action="https://unknownbooks.us18.list-manage.com/subscribe/post?u=520d5322d0f015ca084079162&amp;id=2ccb960521" method="post" id="mc-embedded-subscribe-form" name="mc-embedded-subscribe-form" class="validate" target="_blank" novalidate>
        <div id="mc_embed_signup_scroll">
          <div class="indicates-required"><span class="asterisk">*</span> indicates required</div>
          <div class="mc-field-group">
            <label for="mce-LNAME">姓 </label>
            <input type="text" value="" name="LNAME" class="" id="mce-LNAME">
          </div>
          <div class="mc-field-group">
            <label for="mce-FNAME">名 </label>
            <input type="text" value="" name="FNAME" class="" id="mce-FNAME">
          </div>
          <div class="mc-field-group">
            <label for="mce-EMAIL">メールアドレス  <span class="asterisk">*</span>
            </label>
            <input type="email" value="" name="EMAIL" class="required email" id="mce-EMAIL">
          </div>
          <div class="mc-field-group">
            <label for="mce-PREFECTURE">お住いの地域（47都道府県） </label>
            <input type="text" value="" name="PREFECTURE" class="" id="mce-PREFECTURE">
          </div>
          <div class="mc-field-group">
            <label for="mce-OCCUPATION">職業 </label>
            <input type="text" value="" name="OCCUPATION" class="" id="mce-OCCUPATION">
          </div>
          <div class="mc-field-group">
            <label for="mce-TEXT">質問等備考欄 </label>
            <input type="text" value="" name="TEXT" class="" id="mce-TEXT">
          </div>
          <div id="mce-responses" class="clear">
            <div class="response" id="mce-error-response" style="display:none"></div>
            <div class="response" id="mce-success-response" style="display:none"></div>
          </div>    <!-- real people should not fill this in and expect good things - do not remove this or risk form bot signups-->
          <div style="position: absolute; left: -5000px;" aria-hidden="true"><input type="text" name="b_520d5322d0f015ca084079162_2ccb960521" tabindex="-1" value=""></div>
          <div class="clear"><input type="submit" value="申し込む" name="申し込む" id="mc-embedded-subscribe" class="button"></div>
        </div>
      </form>
    </div>
    <!--End mc_embed_signup-->
  </section>
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
      width: 120px;
      height: auto;
      flex: 0 0 120px;
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
  #mc_embed_signup{background:#fff; clear:left; font:14px Helvetica,Arial,sans-serif; }
</style>
