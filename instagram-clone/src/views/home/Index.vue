<template>
  <div class="home">
    <h1>home</h1>
    <CustomText tag="p">merhaba dunya</CustomText>
    <CustomText class="a1" tag="p" size="small">naber dunya</CustomText>
    <CustomText class="a2" tag="p" size="xsmall">naber dunya</CustomText>
    <CustomText class="a3" tag="p" size="xxsmall">naber dunya</CustomText>
    <IconHome width="60" height="60"/>
  </div>
</template>

<script>
import CustomText from "@/components/CustomText"
import IconHome from '@/icons/home.svg'

export default {
  name: "Index",
  components : {
    CustomText,
    IconHome
  }
}
</script>
<style scoped>
/* h1 {
  color: red;

  @media (--t) {
    color: blue;
  } */
  /* burada post css config i çalıştı, tablet modund ayani çöznürlük değiştiğinde renk değişecek */
/* } */
.a1{
  color : rgba(var(--edc, 150,230,50),1)
}
.a2{
  color : rgba(var(--j64),1)
}
.a3{
  color : rgba(var(--f52),1)
}
</style>
