<template>
  <section class="sect-card">
      <div class="top-title">
          <h6>JOIN MAXCOACH AT BEST</h6>
          <h3>Latest Online <span>Courses</span></h3>

      </div>
      <div class="cards">
          <div class="card" v-for="cards, index in card" :key="index">
              <img :src="require('../assets/img/' + cards.img)" alt="">
              <span class="price">{{cards.price}}</span>
              <h6>{{cards.text}}</h6>
              <span><i class="fa-solid fa-desktop"></i> {{cards.lessons}} Lessons  </span>
              <span><i class="fa-regular fa-circle-user"></i> {{cards.students}} Students</span>
          </div>
          
      </div>
      <div class="selection">
        <ul>
            <li>.</li>
            <li class="point-grey">.</li>
            <li class="point-grey">.</li>
            <li class="point-grey">.</li>
            <li class="point-grey">.</li>
        </ul>
        <p>Control your personal preference settings to get notified about appropriate courses. <span>View all courses <i class="fa-solid fa-arrow-right"></i></span></p>
      </div>
  </section>
</template>

<script>
export default {
name:"MyThirdSection",
props: {
        card: Array,
    },
}
</script>

<style lang="scss">
    .sect-card{
        background-color: rgb(242, 237, 237);
        margin-top: 25px;
    }
    .top-title{
        margin-top: 80px;
        margin-bottom: 30px;
        text-align: center;
        background-color: white;
        h6{
            color:darkgray;
            font-size: 8px;
            margin-bottom: 15px;
        }
        span{
            color: #1fad95;
            
        }

    }
.cards{
    width: 80%;
    margin: auto;
    display: flex;
    margin-top: 35px;
    

    .card{
        width:30%;
        height:200px;
        margin-right: 4%;
        background-color: white;
        padding-bottom: 15px;
        .price{
            color: #1fad95;
            margin:5px 10px;
            font-size: 10px;
        }
        h6{
            padding:8px;
        }

        img{
            height: 60%;
            width: 100%;
        }
        span,i{
            font-size: 10px;
            color: darkgray;
        }
        i{
            margin:0 7px;
        }
        
        }
        
    }
    .selection{
            margin:15px auto ;
            width: 300px;
            text-align: center;
            
            span{
                color:black;
            }
            p{
                font-size: 9px;
                color:rgb(129, 126, 126);
                padding-bottom: 50px;
            }
            li{
                display: inline-block;
                padding: 10px;
                font-size: 30px;
                
            }
            .point-grey{
                    color: lightgray;
                }
        }

</style>