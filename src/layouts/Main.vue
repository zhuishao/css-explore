<template>
  <div class="container">
    <ul style="position: fixed; width: 256px;">
      <li>
        <v-link href="/" accesskey="`">简介</v-link>
      </li>
      <li>
        <v-link href="/buttonOne" accesskey="1">Button-1</v-link>
      </li>
      <li>
        <v-link href="/buttonTwo" accesskey="2">Button-2</v-link>
      </li>
      <li>
        <v-link href="/fontOne" accesskey="3">Font-1</v-link>
      </li>
      <li>
        <v-link href="/fontTwo" accesskey="4">Font-2</v-link>
      </li>
      <li>
        <v-link href="/background" accesskey="5">BackgroundOne</v-link>
      </li>
      <li>
        <v-link href="/backgroundTwo" accesskey="6">BackgroundTwo</v-link>
      </li>
      <li v-show="false">
        <v-link href="/rotate">rotate</v-link>
      </li>
      <li v-show="false">
        <v-link href="/triangleMove" accesskey="7">triangleMove</v-link>
      </li>
    </ul>
    <article><slot></slot></article>
  </div>
</template>

<script>
  import VLink from '../components/VLink.vue'

  export default {
    components: {
      VLink
    }
  }
</script>

<style scoped lang="less">
  @keyframes move {
    0%{
      padding-left: 100%;
      opacity: 0;
    }
    100%{
      padding-left: 0;
      opacity: 1;
    }

  }
  .container {
    background-color: rgb(33,6,114);
    display: flex;
    min-height: 100vh;
    ul{
      flex:none;
      width: 300px;
      li{
        font-size: 40px;
        list-style-type: none;
        white-space: nowrap;
        margin-top:1em;
        overflow: hidden;
        a{text-decoration: none;}
      }
      li:nth-of-type(1){
        animation: move 1.2s;
      }
      li:nth-of-type(2){
        animation: move 1.2s .1s;
      }
      li:nth-of-type(3){
        animation: move 1.2s .2s;
      }
      li:nth-of-type(4){
        animation: move 1.2s .3s;
      }
      li:nth-of-type(5){
        animation: move 1.2s .4s;
      }
      li:nth-of-type(6){
        animation: move 1.2s .5s;
      }
      li:nth-of-type(7){
        animation: move 1.2s .6s;
      }
    }
    article{
      flex: 1;
      background-color: rgb(136,110,215);
    }
  }
</style>
