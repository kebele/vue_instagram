<template>
  <div class="home">
    <div class="timeline">
      <h1>home</h1>
      <!-- <Avatar size="80"></Avatar> bunu Post.vue ya taşıdım -->
      <br />
      <br />
      <br />
      <br />
      <Post></Post>

      <br />
      <br />
      <br />
      <br />
    </div>
    <div class="sidebar">
      <p>
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. At dolorem
        assumenda facere, error omnis ratione dicta quae deleniti architecto
        doloremque nesciunt voluptate quo saepe quidem dolore, aliquid ut. Odio
        dolores quae sed quibusdam similique perferendis explicabo eveniet.
        Iure, aperiam totam repellendus quaerat harum earum, omnis consequatur
        aspernatur aliquid neque ullam.
      </p>
    </div>
  </div>
</template>

<script>
// import CustomText from "@/components/CustomText"
// import IconHome from '@/icons/home.svg'
// import Avatar from '@/components/Avatar'
import Post from "@/components/Post";

export default {
  name: "Home",
  components: {
    // CustomText,
    // IconHome,
    // Avatar,
    Post,
  },
};
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
.home {
  max-width: 605px;
  margin-left: auto;
  margin-right: auto;
  @media (--t) {
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
