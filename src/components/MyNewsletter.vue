<template>
  <section>
    <div class="news">
        <div class="sub">
            <h3>Subscribe <span>Newsletters</span></h3>
            <p>Enter your mail address to register to our newsletter subscription delivered on a regular basis!</p>
            <button class="mail">Enter your email</button><button class="reg">Subscribe</button>
        </div>
        <div class="news-right">
            <div class="up">
                <img src="../assets/img/maxcoach-shape-02.png" alt="">
            </div>
            <div class="down">
                <img src="../assets/img/maxcoach-shape-09.png" alt="">
            </div>
        </div>
    </div>
  </section>
</template>

<script>
export default {
name:"MyNewsletter"
}
</script>

<style lang="scss">
.news{
    width:60%;
    margin: 0 auto;
    display: flex;
    text-align: center;
    padding: 30px 0px;
    h3{
        margin: 15px 25px;
    }
    .mail{
        font-size: 9px;
        width:280px;
        padding: 5px 200px 5px 5px;
        border:0px
    }
    .reg{
        font-size: 10px;
        background-color: #1fad95;
        border: 0px;
        padding:5px 30px 5px 30px;
        color: white;
        margin-bottom: 50px;
        margin-top: 20px;
    }
    p{
        margin: 25px 15px;
        padding: 0 25px;
        font-size: 10px;
    }
    span{
        color: #1fad95;
    }
    .sub{
        width: 85%;
    }
    .news-right{
        width: 15%;
        position: relative;
        .up{
            position: absolute;
            z-index: 999;
            left:50%;
            top:30%;
            width:50px;
        }
    }
}
</style>