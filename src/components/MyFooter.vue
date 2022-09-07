<template>
  <footer>
      <div class="foot-left">
          <h6>Address</h6>
          <span>382 NE 191st # 87394 Miami, FL 33179 - 3899</span>
          <span>+1(305)547-9909(9am - 5pm EST,Mnday - Friday)</span>
          <a href="#">support@maxcoach.com</a>
          <div class="social">
            <a href="#"><i class="fa-brands fa-square-facebook"></i></a>
          <a href="#"><i class="fa-brands fa-twitter"></i></a>
          <a href="#"><i class="fa-brands fa-square-instagram"></i></a>
          <a href="#"><i class="fa-brands fa-invision"></i></a>
          </div>
          

      </div>
      <div class="foot-right">
          <div class="explore">
              <h6>Explore</h6>
              <ul v-for="link, index in link" :key="index">
                  <li>
                      <a :href="link.href">{{link.text}}</a>
                  </li>
              </ul>
          </div>
          <div class="cntr">
              <ul v-for="middle, index in middle" :key="index">
                  <li>
                      <a :href="middle.href">{{middle.text}}</a>
                  </li>
              </ul>
          </div>
          <div class="information">
              <h6>Information</h6>
              <ul v-for="information, index in information" :key="index">
                  <li>
                      <a :href="information.href">{{information.text}}</a>
                  </li>
              </ul>
          </div>
      </div>
  </footer>
</template>

<script>
export default {
name:"MyFooter",
props: {
        information: Array,
        middle:Array,
        link:Array
    },
}
</script>

<style lang="scss">
footer{
    display: flex;
    background-color: black;
    height: 300px;
    .foot-left{
        width:50%;
        span{
            display: block;
            font-size: 9px;
            color: darkgray;
            margin: 10px 10px;
        }
        a{
            text-decoration: none;
            color: darkgray;
            margin: 10px 10px;
        }
        h6{
            color: white;
            margin: 30px 10px;
        }
        .social{
            margin: 10px 10px;
        }
    }
    .foot-right{
        display: flex;
        h6{
            color:white;
            margin:30px 0px;
        }
        a{
            text-decoration: none;
            color: darkgray;
            font-size: 9px;
        }
        .explore{
            width: 30%;
            margin-right: 40px;
        }
        .cntr{
            width: 30%;
            margin-right: 40px;
            padding-top: 73px;
            
        }
        .information{
            width: 30%;
        }
    }
}
</style>