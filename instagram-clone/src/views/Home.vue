<template>
  <div class="home">
   <h1>home</h1>
    
  </div>
</template>

<script>


export default {
  name: "Home",
  
};
</script>
<style scoped>
  h1{
    color : red;

    @media (--t) {
      color : blue;
    }
    /* burada post css config i çalıştı, tablet modund ayani çöznürlük değiştiğinde renk değişecek */
  }
</style>