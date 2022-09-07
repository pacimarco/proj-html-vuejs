<template>
  <section>
      <div class="test-container">
        <div class="test-left">
            <h6>TESTIMONIALS</h6>
            <h3>
                Why do People <span>*Heart*</span> Us?
            </h3>
            <p>Seeking for verbals of our service quality? Find them here. Everything is trasparent and straightfoward for your sense of justification.</p>
            <a href="#">View All<i class="fa-solid fa-arrow-right"></i></a>
        </div>
        <div class="test-right">
            <div class="info-card">
                <h5>Professional team of specialists and passionate mentors at reach</h5>
                <p>I need to get a certification for English profiency and MaxCoach is my best choice. Their tutors are smart and professional when dealing with students.</p>
                <div class="mini-card" v-for="office, index in info" :key="index">
                    <div class="test-img">
                        <img :src="require('../assets/img/' + office.img)" alt="">
                    </div>
                    <div class="position">
                        <h4>{{office.name}}</h4>
                        <h5>/{{office.prov}}</h5>
                    </div>
                </div>
            </div>
            
        </div>
    </div>
  </section>
</template>
<!--     
<div class="sup">
                <h5>Professional team of specialists and passionate mentors at reach</h5>
                <p>I need to get a certification for English profiency and MaxCoach is my best choice. Their tutors are smart and professional when dealing with students.</p>
                <div class="mini-card">
                    <div class="test-img"></div>
                    <div class="position">
                        <h4></h4>
                        <h5>/</h5>
                    </div>
                </div>
            </div>

-->
<script>
export default {
name:"MyTestimonials",
props: {
        info: Array,
    },
}
</script>

<style lang="scss">
.test-container{
    display: flex;
    width: 80%;
    margin:50px auto;

    .test-left{
        width: 35%;
        h6{
            color: darkgray;
            font-size: 9px;
            margin:15px 5px;
        }
        span{
            color: #1fad95;
        }
        h3{
            margin: 15px 5px;
        }
        p{
            margin:15px 5px;
            font-size: 9px;
            color:darkgray;
        }
        a{
            text-decoration: none;
            color:black;
            margin: 15px 5px;
            font-size: 10px;
        }
    }
    .test-right{
        width: 60%;
        .info-card{
            h5{
                margin:15px 5px;
            }
            p{
                margin:15px 5px;
                font-size: 9px;
                color:darkgray;
            }
        }
    }
    .mini-card{
        display: flex;
        img{
            border-radius: 100px;
            
        }
    }
}
.position{
    margin:80px 15px;
}
</style>