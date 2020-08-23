<template>
  <div class="home">
    <CustomText tag="h1">profile</CustomText>

    <router-view></router-view>
    <div id="nav">
      <router-link to="/profile">Post</router-link> |
      <router-link to="/profile/igtv">IGTV</router-link> |
      <router-link to="/profile/save">Save</router-link> |
      <router-link to="/profile/tag">Tag</router-link>
    </div>
  </div>
</template>

<script>
import CustomText from "@/components/CustomText";

export default {
  name: "ProfilePost",
  components: {
    CustomText,
  },
};
</script>
<style scoped></style>
