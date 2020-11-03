<template>
  <div>

  <div class="girl-lk-header">
    <el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" >
  <el-menu-item index="1"><nuxt-link to="/girl-lk">МОЙ ПРОФИЛЬ</nuxt-link></el-menu-item>
  <el-menu-item index="2"><nuxt-link to="/girl-lk-chat">МОИ ЧАТЫ</nuxt-link></el-menu-item>
  <el-menu-item index="3"><nuxt-link to="/girl-lk-streams">МОИ ТРАНСЛЯЦИИ</nuxt-link></el-menu-item>
  <el-menu-item index="4"><nuxt-link to="/girl-lk">МОИ ДРУЗЬЯ</nuxt-link></el-menu-item>

</el-menu>
<div class="line"></div>
    <div class="girl-lk-header__right">
      <el-tag style="margin-right: 20px" effect="plain" type="info">5000 B</el-tag>
       <el-button icon="el-icon-bell" circle></el-button>
       <el-button icon="el-icon-chat-line-round" circle></el-button>
    </div>
  </div>
<div class="container">
   <p class="section-subheader  mb-40">ТРАНСЛЯЦИИ</p>
<el-collapse  class="mb-40">
  <el-collapse-item title="ИНСТРУКЦИЯ ПО ЗАПУСКУ ТРАНСЛЯЦИИ " name="1">
    <div>Lorem ipsum dolor.</div>
    <div>Lorem ipsum dolor.</div>
    <div>Lorem ipsum dolor.</div>
    <div>Lorem ipsum dolor.</div>
    <div>Lorem ipsum dolor.</div>
    <div>Lorem ipsum dolor.</div>
    <div>Lorem ipsum dolor.</div>
    <div>Lorem ipsum dolor.</div>
    <div>Lorem ipsum dolor.</div>
    <div>Lorem ipsum dolor.</div>

  </el-collapse-item>

</el-collapse>
     <p class="section-subheader  mb-40">ЗАПЛАНИРОВАННЫЕ ТРАНСЛЯЦИИ</p>

  <div class="girl-lk-streams">
    <div class="girl-lk-streams__add"><p>Добавить</p></div>
    <div class="girl-lk-streams__inner">
      <div class="girl-lk-streams__item">
        <img src="http://placehold.it/360x180" alt="">
        <p>Тема</p>
        <p>Дата</p>
      </div>
       <div class="girl-lk-streams__item">
        <img src="http://placehold.it/360x180" alt="">
        <p>Тема</p>
        <p>Дата</p>
      </div>
       <div class="girl-lk-streams__item">
        <img src="http://placehold.it/360x180" alt="">
        <p>Тема</p>
        <p>Дата</p>
      </div>
    </div>
  </div>

</div>








  </div>
</template>

<script>

  export default {
    layout: 'login',
    data(){
      return {
        value1:'',
        value2:'',
        activeIndex: '3',
      }
    },

  }
</script>


<style>
.el-menu.el-menu--horizontal {
  border-bottom: none;

}
  .el-collapse-item__header{
    background: transparent;
  }
  .el-collapse-item__wrap{
    background: transparent;
  }
</style>
