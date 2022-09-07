<template>
  <section>
      <div class="trasf-container">
          <div class="trasf-card" v-for="photo, index in picture" :key="index">
            <img class="top" :src="require('../assets/img/' + photo.img)" alt="">
            <img class="max" src="../assets/img/maxcoach-shape-01.png" alt="">
            <img class="shape" src="../assets/img/maxcoach-shape-05-150x150.png" alt="">
          </div>
          <div class="trasf-right">
            <i class="fa-regular fa-circle"></i>
            <h6>EVERYTHING IN <span>MAXCOACH</span></h6>
            <h3>We're Here To <span>Trasform</span> You</h3>
            <p>As learners, people can enjoy great companionship from MaxCoach mentors and educators. We can help you develop and grow at your best.</p>
            <button>Get Free Guide</button>
        </div>
      </div>
  </section>
</template>

<script>
export default {
name:"MyTrasform",
props: {
        picture: Array,
    },
}
</script>

<style lang="scss">
.trasf-container{
    width:80%;
    margin: auto;
    display: flex;
    margin-top: 25px;
    .trasf-card{
        width: 60%;
        position: relative;
    }
    .trasf-right{
        width:35%;
        i{
            color: #febc4d;
        }
        h6{
            font-size: 9px;
            color: lightgray;
            margin:15px 5px;
                
            
            span{
                color:black
            }
        }
        h3{
            margin:15px 5px;
            span{
                color: #1fad95;
            }
        }
        p{
            margin:15px 5px;
            font-size: 9px;
            color: darkgray;
        }
        button{
            margin:15px 5px;
            background-color: #1fad95;
            color: white;
            padding: 5px;
            border: 0px;
            font-size: 10px;
            width: 90px;
        }
    }
}
.top{
    z-index: 999;
}
.max{
    width: 60px;
    position: absolute;
    left:-30px;
    top:90%;
}
.shape{
    position: absolute;
    left:-80px;
    z-index: 1;
    top:30%;
}
</style>