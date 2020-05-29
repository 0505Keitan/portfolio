<template>
  <div class="container">
    <div class="box">
      <cardImg class="card" title="Scoreboard" tags="nodejs"  description="さまざまな場面で利用できるスコアボードです。2つ以上デバイスを用意するだけで簡単に利用ができます。" link="https://keitan-node.herokuapp.com/" img="static/scoreboard.png"/>
      <card class="card" title="「ポ」「プ」「テ」「ピ」「ッ」「ク」をランダムに出力して「ポプテピピック」が完成したら竹●房を破壊するjs" tags="JavaScript"  description="タイトルの通りです。" link="https://toliner.github.io/gen_pptp/"/>
      <card class="card" title="Twitcasting Discord Commenter" tags="nodejs" description="ツイキャスのコメントをエンターで送信できないのでDiscordからコメントできるようにするやつです。" link="https://github.com/0505Keitan/twitcasting-discord-commenter"/>
      <cardImg class="card" title="Engineer's Life" tags="LINEスタンプ" description="LINEスタンプです。" link="https://line.me/S/sticker/6863891" img="https://stickershop.line-scdn.net/stickershop/v1/product/6863891/LINEStorePC/main.png"/>
      <cardImg class="card" title="Yasashi Kakumei Labo Tweet Client" tags="PHP" description="やさしいかくめいラボ運営用のツイートクライアントでした。" link="https://twitter.com/yasashikakumei" img="https://0505keitan.com/archive/web/images/yasashiikakumeilab.jpg"/>
      <cardImg class="card" title="このサイト" tags="Vuejs" description="初めてVuejs使いました。" link="#"/>
    </div>
  </div>
</template>

<script>
import card from "@/components/Card"
import cardImg from "@/components/Card-img"

export default {
  components: {
    card,
    cardImg
  },
}
</script>

<style scoped>
.card {
  width: 80%;
  max-width: 500px;
}
</style>
<style>
body {
  background-color: #e9ffe0; }
.container {
  padding: 20px;
  grid-column: 2; }
.box {
  column-width: 400px; }
</style>