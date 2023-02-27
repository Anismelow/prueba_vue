<template>
  <div id="app">
  <HeaderComponent></HeaderComponent>
  <SliderComponent></SliderComponent>
  <div class="center" >
    <LastArticle></LastArticle>
  <SideBar></SideBar>

</div>
</div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue'
import SliderComponent from './components/SliderComponent'
import SideBar from './components/SideBar'

import LastArticle from './components/LastArticle.vue'

export default {
  name: 'App',
  components: {
    HeaderComponent,
    SliderComponent,
    LastArticle,
    SideBar,

  }
}
</script>

<style>
  @import './assets/css/style.css';
</style>
