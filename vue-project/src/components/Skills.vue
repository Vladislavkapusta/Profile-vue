<script>

  export default{
    
    data(){
      return{
        langs:[
        {name:'HTML5', stars: 4, img: 'image-1.png'},
        {name:'CSS3', stars: 3, img: 'image-2.png'},
        {name:'Javascript', stars: 4, img: 'image-3.png'},
        {name:'React', stars: 4, img: 'image-4.png'}
      ]
      }
    }
  }
</script>

<template>
    <div class="skills-space">
        <h1 class="title">Skills</h1>
        <p class="info">I work in such technologies as</p>
        <div class="card-space">
            <div v-for="lang in langs" class="card">
                <img :src='`src/images/${lang.img}`' alt="lang">
                <h3 class="name">{{ lang.name }}</h3>
                <div class="stars-space">
                    <span 
                        v-for="(elem, ind) in Array(5)" 
                        :class="(ind+1 <= lang.stars) ? 'fa fa-star star' : 'fa fa-star deactive star'">
                    </span>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>

    img{
        width: 88px;
        height: 88px; 
    }

    .skills-space{
        height: 400px;
        padding-top: 50px;
        padding-bottom: 50px;
        display: flex;
        flex-direction: column;
        /* align-items: center; */
        justify-content: space-around;
    }
    .card-space{
        display: flex;
        flex-direction: row;
        justify-content: space-around;

        flex-wrap: wrap;
    }

    .card{
        width: 120px;
        display: flex;
        flex-direction: column;

        align-items: center;
    }
    .deactive{
        color: gray
    }
    .stars-space{
        margin-top: 40px;
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        width: 120px;
    }

    .star{
        widows: 26px;
        height: 26px;
    }
    .name{
        color: #828282;
        text-align: center;
        font-family: Abel;
        font-size: 14px;
        font-style: normal;
        font-weight: 400;
        line-height: normal; 
    }
</style>