<script>
import Header from './components/Header.vue';
import Profile from './components/Profile.vue';
import About from './components/About.vue'
import Skills from './components/Skills.vue';
  export default{
    components:{
      Header, Profile, About, Skills
    }
  }
</script>

<template>
  <div class="content">
    <Header></Header>
    <Profile></Profile>
    <About></About>
    <Skills></Skills>
  </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Abel&display=swap');

  .content{
    max-width: 1445px;
    margin-left: auto;
        margin-right: auto;
        height: 100%;
  }

  .title{
        color: var(--Black, #070707);
        text-align: center;
        font-family: Abel;
        font-size: 34px;
        font-style: normal;
        font-weight: 400;
        line-height: normal; 

        margin-bottom: 17px;
    }

    .info{
        color: var(--Black, #070707);
        text-align: center;
        font-family: Abel;
        font-size: 18px;
        font-style: normal;
        font-weight: 400;
        line-height: normal; 

        margin-bottom: 20px;
    }

  *{
    font-family: Abel;
    font-style: normal;
    font-weight: 400; 
  }



</style>
