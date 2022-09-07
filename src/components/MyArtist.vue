<template>
  <section class="artists">
    <div class="artist-title">
          <h6>READ FOR MORE JOYMENT</h6>
          <h3>Latest From <span>Our Bags</span></h3>

      </div>
      <div class="artist-cards">
          <div class="artist-card" v-for="poster, index in artists" :key="index">
              <img :src="require('../assets/img/' + poster.img)" alt="">
              <span class="art">{{poster.title}}</span>
              <h6>{{poster.text}}</h6>
              <span><i class="fa-solid fa-desktop"></i> {{poster.date}}  </span>
              <span><i class="fa-regular fa-circle-user"></i> {{poster.views}} views</span>
          </div>
        </div>
  </section>
</template>

<script>
export default {
name:"MyArtist",
props: {
        artists: Array,
    },
}
</script>

<style lang="scss">
.artist-title{
        margin-top: 80px;
        text-align: center;
        padding-top: 50px;
        h6{
            color:darkgray;
            font-size: 8px;
            margin-bottom: 15px;
        }
        span{
            color: #1fad95;
            
        }

    }
    .artist-cards{
    width: 80%;
    margin: auto;
    display: flex;
    margin-top: 15px;
    padding-bottom: 30px;
    

    .artist-card{
        width:30%;
        height:200px;
        margin-right: 4%;
        background-color: white;
        padding-bottom: 30px;
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
    .art{
        margin:5px 10px;
    }
    .artists{
        background-color: rgb(242, 237, 237);
    }
</style>