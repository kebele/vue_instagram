<template>
  <div class="home">

    <div class="timeline">

    <h1>home</h1>
    <CustomText tag="p">merhaba dunya</CustomText>
    <CustomText class="a1" tag="p" size="small">naber dunya</CustomText>
    <CustomText class="a2" tag="p" size="xsmall">naber dunya</CustomText>
    <CustomText class="a3" tag="p" size="xxsmall">naber dunya</CustomText>
    <IconHome width="60" height="60"/>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Animi culpa unde, autem cupiditate architecto in, illo voluptatem ipsam suscipit labore ex aliquam! In excepturi praesentium, eum vel expedita quam. Officiis, reiciendis deserunt fugiat, perspiciatis velit nobis esse rem doloribus id vitae excepturi. A, pariatur necessitatibus autem magni ab totam eius.</p>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Animi culpa unde, autem cupiditate architecto in, illo voluptatem ipsam suscipit labore ex aliquam! In excepturi praesentium, eum vel expedita quam. Officiis, reiciendis deserunt fugiat, perspiciatis velit nobis esse rem doloribus id vitae excepturi. A, pariatur necessitatibus autem magni ab totam eius.</p>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Animi culpa unde, autem cupiditate architecto in, illo voluptatem ipsam suscipit labore ex aliquam! In excepturi praesentium, eum vel expedita quam. Officiis, reiciendis deserunt fugiat, perspiciatis velit nobis esse rem doloribus id vitae excepturi. A, pariatur necessitatibus autem magni ab totam eius.</p>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Animi culpa unde, autem cupiditate architecto in, illo voluptatem ipsam suscipit labore ex aliquam! In excepturi praesentium, eum vel expedita quam. Officiis, reiciendis deserunt fugiat, perspiciatis velit nobis esse rem doloribus id vitae excepturi. A, pariatur necessitatibus autem magni ab totam eius.</p>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Animi culpa unde, autem cupiditate architecto in, illo voluptatem ipsam suscipit labore ex aliquam! In excepturi praesentium, eum vel expedita quam. Officiis, reiciendis deserunt fugiat, perspiciatis velit nobis esse rem doloribus id vitae excepturi. A, pariatur necessitatibus autem magni ab totam eius.</p>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Animi culpa unde, autem cupiditate architecto in, illo voluptatem ipsam suscipit labore ex aliquam! In excepturi praesentium, eum vel expedita quam. Officiis, reiciendis deserunt fugiat, perspiciatis velit nobis esse rem doloribus id vitae excepturi. A, pariatur necessitatibus autem magni ab totam eius.</p>

    </div>
    <div class="sidebar">
      <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. At dolorem assumenda facere, error omnis ratione dicta quae deleniti architecto doloremque nesciunt voluptate quo saepe quidem dolore, aliquid ut. Odio dolores quae sed quibusdam similique perferendis explicabo eveniet. Iure, aperiam totam repellendus quaerat harum earum, omnis consequatur aspernatur aliquid neque ullam.</p>
      <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. At dolorem assumenda facere, error omnis ratione dicta quae deleniti architecto doloremque nesciunt voluptate quo saepe quidem dolore, aliquid ut. Odio dolores quae sed quibusdam similique perferendis explicabo eveniet. Iure, aperiam totam repellendus quaerat harum earum, omnis consequatur aspernatur aliquid neque ullam.</p>
    </div>

  </div>
</template>

<script>
import CustomText from "@/components/CustomText"
import IconHome from '@/icons/home.svg'

export default {
  name: "Home",
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
/* .a1{
  color : rgba(var(--edc, 150,230,50),1)
}
.a2{
  color : rgba(var(--j64),1)
}
.a3{
  color : rgba(var(--f52),1)
} */
.home{
  max-width: 605px;
  margin-left: auto;
  margin-right: auto;
  @media (--t){
    max-width: none;
    display: grid;
    grid-template-columns: 1fr 295px;
    grid-gap: 30px;
    
  }
}

.sidebar {
  display: none;
  @media (--t) {
    display: block;
  }
}
</style>
