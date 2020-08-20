<template>
  <div class="home">
    <h1>home</h1>
    <CustomText>selam dunya</CustomText>
    <CustomText tag="p">selam dunya</CustomText>
  </div>
</template>

<script>
import CustomText from "@/components/CustomText"
export default {
  name: "Home",
  components : {
    CustomText
  }
}
</script>
<style scoped>
h1 {
  color: red;

  @media (--t) {
    color: blue;
  }
  /* burada post css config i çalıştı, tablet modund ayani çöznürlük değiştiğinde renk değişecek */
}
</style>
