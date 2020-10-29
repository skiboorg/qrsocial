<template>
  <header class="header" >
   <div class="header-wrapper">
       <nuxt-link to="/">
     <div class="logo">
       <img src="/logo.png" alt="">
     </div>
       </nuxt-link>
     <div class="header-nav">
       <ul class="header-nav__wrapper">
         <li class="header-nav__item">
           <nuxt-link class="header-nav__link" to="/girls">我们的女孩</nuxt-link>

         </li>
         <li class="header-nav__item"><nuxt-link class="header-nav__link" to="/groups">社会团体</nuxt-link></li>
         <li class="header-nav__item"><nuxt-link class="header-nav__link" to="/streams">我们的广播</nuxt-link></li>
         <li class="header-nav__item"><a class="header-nav__link" href="#">广播类别</a></li>
       </ul>
     </div>
     <div class="header-balance">
       <div class="header-balance__img">
         <img  src="/header_balance_icon.png" alt="">
       </div>
       <p class="header-balance__amount">2350</p>
       <p class="header-balance__text">我的余额</p>
     </div>
     <div class="header-buttons">
       <div class="header-buttons__item gold-bg">
         <img draggable="false" src="/header_btn_icon1.png" alt="">
       </div>
       <div class="header-buttons__item ">
         <img draggable="false" src="/header_btn_icon2.png" alt="">
       </div>
        <div class="header-buttons__item ">
         <img draggable="false" src="/header_btn_icon3.png" alt="">
       </div>
        <div class="header-buttons__item ">
         <img draggable="false" src="/header_btn_icon4.png" alt="">
       </div>
     </div>
      <nuxt-link to="/profile">
     <div class="btn btn-blue btn-w-img">
         <img src="/header_auth_btn.png" alt="">
       <p>登录或注册</p>
     </div>
    </nuxt-link>
   </div>
  </header>
</template>

<script>
  export default {

    data() {
      return {



      };
    },

    watch: {

    },
    mounted() {

    },
    methods: {


    }
  }
</script>


