<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <!-- <router-link to="/about">About</router-link> -->
      <router-link to="/direct">direct</router-link> |
      <router-link to="/explore">explore</router-link> |
      <router-link to="/profile">profile</router-link>
    </div>
    <router-view />
  </div>
</template>


