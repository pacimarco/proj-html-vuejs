<template>
  <header>
      <div class="container">
          <div class="navbar">
              <!-- MENU LINK -->
              <div class="link">
                    <a :href="item.link" v-for="item, index in headerLinks" :key="index">{{item.text}}  </a> 
              </div>
              <!-- LOGO -->
              <div class="logo">
                    <img src="../assets/img/dark-logo.png" alt="Logo Icademy">
                </div>
                <!-- ICONS -->
                <div class="icons">
                    <i class="fa-solid fa-cart-shopping"></i>
                    <i class="fa-regular fa-circle-user"></i>
                    <div class="circle shop-circle">0</div>
                    <input type="text" placeholder="Search..">
                </div>
          </div>
          <!-- FINE NAVBAR -->
          <!-- jumbo -->
          <div class="jumbo">
              <div class="title-center">
                  <h4>Commence business</h4>
                  <h2>Distant Mentoring Program</h2>
                  <div class="btn jumbo-btn"><a href="#">Download free guidebook <i class="fa-solid fa-arrow-right"></i></a></div>
              </div>
              <div class="lat-icon">
                  <a href="#"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
                  <a href="#"><i class="fa-regular fa-circle"></i></a>
                <a href="#"><i class="fa-solid fa-cart-shopping"></i></a>
                <a href="#"><i class="fa-solid fa-desktop"></i></a>
              </div>
          </div>
      </div>
  </header>
</template>

<script>
export default {
    name:"MyHeader",
    props: {
        headerLinks: Array,
    },

}
</script>

<style lang="scss">
    .navbar{
        display: flex;
        justify-content: space-around;
        align-content: center;
        height: 35px;
        align-items: center;
    }
    .logo{
        width: 100px;
        img{
            width: 100%;
        }
    }
    .link a{
        text-decoration: none;
        color: black;
        padding: 0 10px;
        font-size: 10px;
    }
    .icons{
        display: flex;
        justify-content: space-between;
        width: 210px;
        align-content: center;
    }
    .jumbo{
        position: relative;
        height: 400px;
        background-image: url('../assets/img/home-3-hero-bg.jpg');
        background-size: cover;
        text-align: center;
        .btn {
    margin: 0 auto;
    
    width: 150px;
    font-size: 10px;
    height: 20px;
    line-height: 20px;
    background-color: white;
    margin-top: 10px;
        a {
        color: #1fad95;
        text-decoration: none;
         }
    }
    .title-center{
        display: flex;
        flex-direction: column;
        align-content: center;
        justify-content: center;
        align-items: center;
        padding-top: 130px;


        h2, h4{
            color: white;
            margin-bottom: 15px;
        }
       
    }
    .lat-icon{
        display: flex;
        flex-direction: column;
        background-color: white;
        width: 20px;
        height: 80px;
        position: absolute;
        right: 0;
        top:150px;
        

        a{
            color: black;
        }
    }
        
    }


</style>