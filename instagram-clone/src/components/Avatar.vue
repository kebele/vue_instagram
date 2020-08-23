<template>
  <figure class="avatar">
    <img :src="src" :alt="alt" :width="size" :height="size" />
  </figure>
</template>

<script>
export default {
  name: "Avatar",
  props: {
    src: {
      type: String,
      default:
        "https://instagram.fesb3-1.fna.fbcdn.net/v/t51.2885-19/s150x150/118255309_118179853130935_754774801536933337_n.jpg?_nc_ht=instagram.fesb3-1.fna.fbcdn.net&_nc_ohc=BUk_HBpNthQAX9nAEjm&oh=dc20022660cc415e8cd66379b7abf50b&oe=5F6D2C78",
    },
    alt: {
      type: String,
    },
    size: {
      type: Number,
    },
  },
};
</script>

<style lang="postcss" scoped>
.avatar {
  display: inline-flex;
  padding: 3px;
  border-radius: 999px;
  background : 
  img {
    border-radius: inherit;
    border : 2px solid white;
  }
}
</style>





