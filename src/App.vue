<template>
  <div id="app">
    <MyHeader :headerLinks="headerLink"/>
    <MyMain/>
    <MyFooter :link="link" :middle="middle" :information="information"/>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue';
import MyMain from './components/MyMain.vue';
import MyFooter from './components/MyFooter.vue';


export default {
  name: 'App',
  components: {
    MyHeader,
    MyMain,
    MyFooter,
  },
  data() {
    return {
      headerLink: [
        {
          text: 'Home',
          link: '#',
        },
        {
          text: 'Pages',
          link: '#',
        },
        {
          text: 'Courses',
          link: '#',
        },
        {
          text: 'Features',
          link: '#',
        },
        {
          text: 'Blog',
          link: '#',
        },
        {
          text: 'Shop',
          link: '#',
        },
      ],
      link:[
        {
          text:'Start here',
          href:'#',
        },
        {
          text:'Blog',
          href:'#',
        },
        {
          text:'About us',
          href:'#',
        }
      ],
      middle:[
      {
          text:'Success story',
          href:'#',
        },
        {
          text:'Courses',
          href:'#',
        },
        {
          text:'Contact us',
          href:'#',
        },
      ],
      information:[
      {
          text:'Membership',
          href:'#',
        },
        {
          text:'Purchase guide',
          href:'#',
        },
        {
          text:'Privacy policy',
          href:'#',
        },
        {
          text:'teams of service',
          href:'#',
        },
      ]
}
  }
}
  
</script>

<style lang="scss">
@import '~@fortawesome/fontawesome-free/css/all.css';

body{
  font-family: sans-serif;
}
*{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

</style>
