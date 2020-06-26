<template>
  <div class="profile">
    <b-row>
      <b-col>
         <img src="../assets/profile.png" alt="" class="my_profile_pic"> 
      </b-col>
      <b-col class="contetnts-profile">
        <ul>
          <li>名前：Togemi</li>
          <li>生活圏：岡山近辺(7月から東京近辺へと移動予定)</li>
          <li style="max-width:400px;">略歴：大学在学中から多くの時間を国外で過ごし、
            自分の事業を起こそうと奮起するが失敗。漠然と持っ
            ていた興味を本格的に始めてみようと28歳からエン
            ジニアを目指し独学を始める。社交的な引きこもり。</li>
        </ul>
      </b-col>
    </b-row>
  </div>
</template>

<style scoped>

  .profile{
        position: absolute;
        top: 10%;
        right: 0;
        bottom: 0;
        left: 0;
        padding: 1.25rem;
  }

  .my_profile_pic{
    width: 17em;
    height: 17em;
    border-radius : 50%;
  }

  .contetnts-profile{
    text-align: left;
    margin: auto;
  }
</style>