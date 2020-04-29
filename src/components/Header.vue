<template>
  <header>
    <div class="logo">
      <img src="../assets/logo.png" alt="">
    </div>
    <div class="title">
      <h1>{{ title }}</h1>
    </div>
    <div class="filler"></div>
  </header><!-- /header -->
</template>


<script>
  export default{
    name: "Header",
  props: {
    title: String
  }
  }
</script>
<style scopep>
header{
  width: 100%;
  height: 60px;
  background: #171717;

  padding: 15px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.logo{
  flex: 1;
}
.logo img{
  height: 50px;
}
.title{
  flex: 3;
}
.title h1{
  color: #f3f3f3;
  font-size: 28px;
  line-height: 60px;
  font-weight: 400;
}
.filler{
  flex: 1
}
</style>
