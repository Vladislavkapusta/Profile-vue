<script>
  export default{

  }
</script>

<template>
    <div class="profile">
        <div class="text-space">
            <h1 class="name">Alex Wylliam</h1>
            <p class="profession">web developer 28 years old, Karaganda</p>
            <p class="language">RU|ENG</p>
        </div>
        <img src="../images/BSPP2266.png" alt="pfp">
    </div>
</template>

<style scoped>
    .profile{
        display: flex;
        flex-direction: column;
    }

    .text-space{
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        align-items: center;

        flex-wrap: wrap;
    }

    .name{
        color: var(--Black, #070707);
        font-family: Abel;
        font-size: 47.339px;
        font-style: normal;
        font-weight: 400;
        line-height: normal; 

        width: 160px;
        height: 118px; 
    }

    .profession{
        color: var(--Black, #070707);
        font-family: Abel;
        font-size: 18px;
        font-style: normal;
        font-weight: 400;
        line-height: normal; 

        width: 205px;
        height: 44px; 
    }

    .language{
        color: #828282;
        font-family: Abel;
        font-size: 16px;
        font-style: normal;
        font-weight: 400;
        line-height: normal;
        
        transform: rotate(270deg);
    }
</style>