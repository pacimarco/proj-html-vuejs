<template>
  <section class="sect-1">
    <div class="text">
        <h6>EVERYTHING IN MAXCOACH</h6>
        <h3>Learn about our <span>Work Culture</span> at MaxCoach</h3>
        <p>Spend some time to visit our website or head office and discover our courses, enrollment procedure, and registration deadline. We're opening new classes every beginning of each month.</p>
        <p>Have questions? <a href="#">Get a free guide <i class="fa-solid fa-arrow-right"></i></a></p>
    </div>
    <div class="only-circle">
        <i class="fa-regular fa-circle"></i>
    </div>
    <div class="img-sect1">
        <div class="creative-circle"></div>
        <div class="green-greed"></div>
        <div class="small-img"></div>
    </div>
  </section>
</template>

<script>
export default {
name:"MyFirstSection",
}
</script>

<style lang="scss">
.img-sect1{
    background-image: url('../assets/img/stock-full-hd-10-ohki1ayywq3cqutettrncduujpoaorifqu4relt2ts.jpg');
    background-size: contain;
    background-repeat: no-repeat;
    margin-top: 60px;
    width: 50%;
    position: relative;
}
.small-img{
    background-image: url('../assets/img/about-us-01-ohkia3qg98rq9vg3s0mn2hkflr1migdqdw370qnegc.jpg');
    width: 150px;
    height: 150px;
    position: absolute;
    z-index: 330;
    right: -110px;
    top:-40px;
    
}
.green-greed{
    background-image: url('../assets/img/maxcoach-shape-07-100x100.png');
    background-size: cover;
    width: 50px;
    height: 50px;
    position: absolute;
    right:20px;
    top:-30px;
    z-index: 200;

}
.sect-1{
    height: 480px;
    width: 80%;
    display: flex;
    margin: 0 auto;
}
.text{
    width: 30%;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;

    p{
        font-size: 12px;
    }

    span{
        color: #1fad95;
        
    }

    a{
        text-decoration: none;
        color: #1fad95;
    }

}
.only-circle{
    width: 15%;
    height: 100%;
    margin-top: 60px;
    i{
        font-size: 60px;
        color: #febc4d;
    }
}
</style>