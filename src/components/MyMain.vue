<template>
  <div class="main-container">
    <MyFirstSection/>
    <MySecondSection/>
    <MyThirdSection :card="card"/>
  </div>
</template>

<script>
    import MyFirstSection from './MyFirstSection.vue'
    import MySecondSection from './MySecondSection.vue'
    import MyThirdSection from './MyThirdSection.vue'
export default {
    name:"MyMain",
    components:{
        MyFirstSection,
        MySecondSection,
        MyThirdSection,
    },
    data() {
    return {
      card: [
        {
            img:'course-02-480x298.jpg',
          price:'$ 40.00',
        text: 'Learning to write as a Professional Author',
          lessons: '20',
          students: '50',
        },
        {
            img:'stock-full-hd-03-480x298.jpg',
          price:'$ 0.00',
        text: 'Customer-centric info-Tech Strategies',
          lessons: '24',
          students: '769',
        },
        {
            img:'stock-full-hd-04-480x298.jpg',
          price:'$ 19.00',
        text: 'Open Programming Courses for Everyone: Phiton',
          lessons: '17',
          students: '62',
        },
        
      ],
}
  }

}
</script>

<style>

</style>