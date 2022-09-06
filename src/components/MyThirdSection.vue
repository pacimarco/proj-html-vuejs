<template>
  <section>
      <div class="top-title">
          <h6>JOIN MAXCOACH AT BEST</h6>
          <h3>Latest Online <span>Courses</span></h3>

      </div>
      <div class="cards">
          <div class="card" v-for="cards, index in card" :key="index">
              <img :src="require('../assets/img/' + cards.img)" alt="">
              <span>{{cards.price}}</span>
              <h6>{{cards.text}}</h6>
              <span>{{cards.lessons}} Lessons</span>
              <span>{{cards.students}} Students</span>
          </div>
          
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
.cards{
    width: 80%;
    margin: auto;

    .card{
        width:30%;
        height:400px;

        img{
            height: 60%;
            width: 100%;
        }
        
        }
    }

</style>