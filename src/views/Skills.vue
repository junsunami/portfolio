<template>
    <div class="skills">
        <b-container fluid="sm" class="mb-5">
            <b-row>
                <b-col>
                    <h2>学習分野</h2>
                    <ul class="list_style">
                        <li>Ruby</li>
                        <li>Ruby on Rails</li>
                        <li>JavaScript</li>
                        <li>Vue.js</li>
                        <li>AWS</li>
                        <li>Docker</li>
                    </ul>
                </b-col>
                <b-col>
                    <h2>学習予定分野</h2>
                    <ul class="list_style">
                        <li>Linuxへの知見を深めたい</li>
                        <li>CI</li>
                        <li>TypeScript</li>
                        <li>Solidity</li>
                    </ul>
                </b-col>
            </b-row>
        </b-container>
        <h1 class="mb-">作ったもの</h1>
        <div class="container">
            <div class="box1">
                <a href="https://incomeapp.ml">
                  <img src="../assets/hourly_wage.png" class="pic_action img-fluid" />
                </a>
                <h3>Railsで作成した<br>時給管理アプリ</h3>
            </div>
            <div class="box2 box">
                    <img src="../assets/portfolio_page.png" class="pic_action img-fluid" />
                    <h3>Vue.jsで作成した<br>簡易ポートフォリオ</h3>
            </div>
            <div class="box3">
                <img src="../assets/404.png" class="pic_action img-fluid" />
                <h3>Vue.jsを利用した<br>SPAを製作予定</h3>
            </div>
        </div>
    </div>
</template>

<style scoped>
    h1,h2{
        margin-bottom: 0.5em;
    }

    h3{
        margin-top:0.5em;
    }

    .skills{
        position: absolute;
        top: 10%;
        right: 0;
        bottom: 0;
        left: 0;
        padding: 1.25rem;
    }

    .list_style{
        list-style: none;
        padding-left: 0;
    }

    .container {
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        grid-row-gap: 10px;
        grid-column-gap: 30px;
    }

    .pic_action:hover{
        width: 100%;
        transform: scale(1.03);
        transition-duration: 1s;
        opacity: 0.8;
    }
</style>