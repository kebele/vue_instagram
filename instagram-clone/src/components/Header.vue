<template>
  <header class="header">
    <Container class="header-inner">
      <!-- logo -->
      <router-link class="logo" to="/">instagram</router-link>
      <!-- <router-link to="/">Home</router-link>  -->

<!-- search -->
      <form class="search">
        <input type="text" placeholder="search" />
      </form>
      <!-- navigation -->
      <nav class="navigation">
        <router-link to="/">
          <IconHomeFill v-if="$route.name === 'Home'"/>
          <IconHome v-else/>
          <!-- eğer route un name i home ise bunu göster, değilse v-else olanı göster, biz başka bir linke tıkladığımızda route.name değişeceği için... -->
        </router-link>
        <!-- <router-link to="/about">About</router-link> -->
        <router-link to="/direct">
            <IconDirectFill v-if="$route.name === 'Direct'"></IconDirectFill>
            <IconDirect v-else></IconDirect>
        </router-link>
        <router-link to="/explore">
            <IconExploreFill v-if="$route.name === 'Explore'"></IconExploreFill>
            <IconExplore v-else></IconExplore>
        </router-link>
        <router-link to="/profile">
          <Avatar size="26"></Avatar>
        </router-link>
      </nav>
    </Container>
  </header>
</template>

<script>
import IconHome from "@/icons/home.svg";
import IconHomeFill from "@/icons/home-fill.svg";
import IconDirect from "@/icons/direct.svg";
import IconDirectFill from "@/icons/direct-fill.svg";
import IconExplore from "@/icons/explore.svg";
import IconExploreFill from "@/icons/explore-fill.svg";
import Avatar from '@/components/Avatar';
import Container from "@/components/Container";

export default {
  name: "MainHeader",
  components: {
    IconHome,
    IconHomeFill,
    IconDirect,
    IconDirectFill,
    IconExplore,
    IconExploreFill,
    Avatar,
    Container,
  },
};
</script>

<style scoped>
.header {
  /* background-color: yellow; */
  z-index: 90;
  position: fixed;
  left: 0;right: 0;top: 0;
  background-color: white;
  border-bottom : 1px solid rgb(var(--b6a));  
  }

.header-inner {
    height: var(--header-height);
    display: flex;
    align-items: center;
    justify-content: center; 

  @media (--t){
    display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  align-items: center;
  }
}
.logo{
    font-size: 1.6rem;
    font-weight: bold;
}
.search{
  display: none;

  @media (--t){
    display : block;
     text-align: center;    

input{
    width: 215px;
    height: 28px;
    border : 1px solid rgb(var(--b6a));
    border-radius : 4px;
    background-color: rgb(var(--b3f));
    padding-left: 20px;
    padding-right: 20px;
}

  }
}

.navigation{
  z-index: 90;
  position: fixed;
  left: 0;
  right: 0;bottom: 0;
  background-color: white;
  border-top : 1px solid rgb(var(--b6a));
  height: 80px;
  display: flex;
  align-items: center;
  justify-content: space-around;

  @media (--t){
    /* position u staticleştir, left,right vs değerlerinin hiç birini okumaz */
    height: auto;
    border : 0;
    position: static;
    /* display: flex; */
    justify-content: flex-end;
    
    a{
        margin-left: 20px;
    } 
  }
     
}


</style>
