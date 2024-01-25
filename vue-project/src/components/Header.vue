<script>
  export default{
    data(){
      return{
        titles:[
          'Home',
          'About me',
          'Skills',
          'Portfolio',
          'Contacts'
      ]
      }
    }
  }
</script>

<template>
  <header>
    <div class="main-space">
      <p v-for="title in titles">
      {{ title }}
      </p>
    </div>
    <div class="header-line"></div>
  </header>
</template>

<style scoped>
  .main-space{
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: space-between;

    margin: 0;
    height: 66px;
  }

  .header-line{
    background-color: #828282; 
    width: 100%;
    height: 1px;
  }
</style>
