<template>
  <div id="app">
    <Header title="VueJS"/>
    <Profile :user="user"/>
  </div>
</template>

<script>
import Header from './components/Header';
import Profile from './components/Profile';
export default {
  name: 'App',
  components: {
    Header,
    Profile
  },
  data: function(){
    return {
      user: {
        name: "Peter Parker",
        image: require("./assets/spider-man.jpg")
      }
    }
  }
}
</script>

<style>
body{
  margin: 0;
  background: #f3f3f3;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
