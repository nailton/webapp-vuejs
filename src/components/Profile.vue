<template>
  <section id="profile">
    <img :src="user.image">
    <h3>{{ user.name }}</h3>
  </section>
</template>

<script>
  export default{
    name: "Profile",
    props: {
      user: Object
    }
  }
</script>

<style scoped="">
  #porfile{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 15px;
  }
  #profile img{
    padding-top: 15px;
    width: 50%;
  }
</style>
