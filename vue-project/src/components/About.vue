<script>
  export default{

  }
</script>

<template>
    <div class="about-space">
        <h1 class="title">About me</h1>
        <p class="info">Hi, I'm Alex – web developer from Karaganda. <br>
I'm interested in development and everything connected with it</p>
        <p class="info"> Ready to implement excellent projects <br> with wonderful people.</p>
    </div>
</template>

<style scoped>
    .about-space{
        height: 500px;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;

        background: #F6F6F6; 
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
</style>