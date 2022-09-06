<template>
  <div id="app">
    <MyHeader :headerLinks="headerLink"/>
    <MyMain/>
    <MyFooter/>
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
