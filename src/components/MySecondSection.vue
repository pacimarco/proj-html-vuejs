<template>
  <section>
      <div class="container-sect-2">
        <div class="left">
            <div class="cover-l">

            </div>
            <div class="youtube-logo">
                <img src="../assets/img/icon-youtube-play.png" alt="youtube">
            </div>
            <div class="cover-r">

            </div>
        </div>
      
        <div class="rigth">
            <h6>HOW WE WORK</h6>
            <h3>Upgrade Your Skills <span>Upgrade Your Life </span></h3>
            <p>Opening up more opportunities in front of you to get the ticket to more enjoyable door in life. Getting equipped with new skills for new sets of insights into your carrer. MaxCoach accompany learners in every stage of learning.</p>
            <a href="#">Download free guidebook <i class="fa-solid fa-arrow-right"></i></a>
        </div>
      </div>
      
  </section>
</template>

<script>
export default {

}
</script>

<style lang="scss">
.container-sect-2{
    width: 80%;
    height: 300px;
    display: flex;
    margin: auto;
    margin-top: 30px;

    .left{
        background-image: url('../assets/img/stock-full-hd-11-670x450.jpg');
        width: 60%;
        position: relative;
       
        .youtube-logo{
            position: absolute;
            top:40%;
            left:40%
        }

        .cover-l{
            width:150px;
            height: 150px;
            background-image: url('../assets/img/maxcoach-shape-05-150x150.png');
            background-repeat: no-repeat;
            position: absolute;
            background-size: cover;
            left:-60px;
            top:30px;
            z-index: -1;
        }
        .cover-r{
            width:150px;
            height: 150px;
            background-image: url('../assets/img/maxcoach-shape-07-150x150.png');
            position: absolute;
            bottom: -40px;
            right:-25px;
            z-index: -1;
        }
    }
    .rigth{
        width: 35%;
        margin-left: 50px;
        
        h3, h6{
            margin-top: 25px;
        }
        span{
            color: #1fad95;
        }
        a{
            color: black;
            
        }
        p{
            color: darkgray;
            margin-top: 25px;
            font-size: 12px;
            margin-bottom: 25px;
        }
    }
}
</style>