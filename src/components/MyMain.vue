<template>
  <div class="main-container">
    <MyFirstSection/>
    <MySecondSection/>
    <MyThirdSection :card="card"/>
    <MyTestimonials :info="info"/>
    <MyTrasform :picture="picture"/>
    <MyArtist :artists="artists"/>
    <MyNewsletter/>
  </div>
</template>

<script>
    import MyFirstSection from './MyFirstSection.vue'
    import MySecondSection from './MySecondSection.vue'
    import MyThirdSection from './MyThirdSection.vue'
    import MyTestimonials from './MyTestimonials.vue'
    import MyTrasform from './MyTrasform.vue'
    import MyArtist from './MyArtist.vue'
    import MyNewsletter from './MyNewsletter.vue'
export default {
    name:"MyMain",
    components:{
        MyFirstSection,
        MySecondSection,
        MyThirdSection,
        MyTestimonials,
        MyTrasform,
        MyArtist,
        MyNewsletter
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
      info:[
          {
              img:'testimonial-avata-02.jpg',
              name:'MINA HOLLACE',
              prov:'Freelancer'
          },
          {
              img:'testimonial-avata-01.jpg',
              name:'MADLEY PONDOR',
              prov:'It Specialist'
          }
      ],
      picture:[
          {
              img:'home-3-team-image-300x278.png',
          }
      ],
      artists:[
          {
            img:'artist-blog-03-480x325.jpeg',
          title:'ARTIST',
          text:'Brush Strokes Energize Trees In Paintings',
          date:'May 15 2020',
          views:'688',
          },
          {
            img:'artist-blog-01-480x325.jpg',
          title:'ARTIST',
          text:'Pocket-Size Notebooks Hold Miniature Paintings',
          date:'May 15 2020',
          views:'603',
          },
          {
            img:'artist-blog-02-480x325.jpg',
          title:'ARTIST',
          text:'Connection Between Self-Portraits and Identity',
          date:'May 15 2020',
          views:'397',
          },
          ],
      }
      
}
  }


</script>

<style>

</style>