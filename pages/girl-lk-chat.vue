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
   <p class="section-subheader  mb-40">Чаты</p>
 <div class="chat-wrapper mb-40">
                <div class="chat-left">
                  <div class="chat-users">
                    <ul>
                      <!--                chatItemActive-->
                      <li class="chat-users__item chatItemActive">
                        <div class="avatarVip">
                           <img class="chat-users__item--img" src="https://picsum.photos/400/400?image=24" alt="">
                        </div>

                        <div class="chat-users__item--lastMsg">
                          <p class="chat-users__item--text">我的简历</p>
                          <p class="chat-users__item--msg">fdgdvbcvbcvb  </p>
                        </div>
                        <p class="chat-users__item--time">10:30 10.09</p>
                      </li>
                      <li class="chat-users__item ">
                        <img class="chat-users__item--img" src="https://picsum.photos/400/400?image=56" alt="">
                        <div class="chat-users__item--lastMsg">
                          <p class="chat-users__item--text">我的简历</p>
                          <p class="chat-users__item--msg">fdgdfgfdg </p>
                        </div>
                        <p class="chat-users__item--time">10:30 10.09</p>
                      </li>
                      <li class="chat-users__item ">
                        <img class="chat-users__item--img" src="https://picsum.photos/400/400?image=53" alt="">
                        <div class="chat-users__item--lastMsg">
                          <p class="chat-users__item--text">我的简历</p>
                          <p class="chat-users__item--msg">fdgdfgfdg </p>
                        </div>
                        <p class="chat-users__item--time">10:30 10.09</p>
                      </li>
                      <li class="chat-users__item ">
                        <img class="chat-users__item--img" src="https://picsum.photos/400/400?image=50" alt="">
                        <div class="chat-users__item--lastMsg">
                          <p class="chat-users__item--text">我的简历</p>
                          <p class="chat-users__item--msg">fdgdfgfdg </p>
                        </div>
                        <p class="chat-users__item--time">10:30 10.09</p>
                      </li>
                      <li class="chat-users__item ">
                        <img class="chat-users__item--img" src="https://picsum.photos/400/400?image=76" alt="">
                        <div class="chat-users__item--lastMsg">
                          <p class="chat-users__item--text">我的简历</p>
                          <p class="chat-users__item--msg">fdgdfgfdg </p>
                        </div>
                        <p class="chat-users__item--time">10:30 10.09</p>
                      </li>

                    </ul>
                  </div>
                </div>
                <div class="chat-right ">
                  <div class="chat-content">
                    <div class="chat-content-msg">
                       <div class="chat-content-msg__item">
<!--                        avatarVip-->
                        <div class="chat-content-msg__item--img avatarVip">
                           <img  src="https://picsum.photos/400/400?image=73" alt="">
                        </div>

                        <p class="chat-content-msg__item--text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium alias animi deleniti laborum modi mollitia repudiandae sint soluta temporibus tenetur?</p>
                        <p class="chat-content-msg__item--time">10:30 10.09</p>
                      </div>
                       <div class="chat-content-msg__item">
<!--                        avatarVip-->
                        <div class="chat-content-msg__item--img avatarVip">
                           <img  src="https://picsum.photos/400/400?image=73" alt="">
                        </div>

                        <p class="chat-content-msg__item--text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium alias animi deleniti laborum modi mollitia repudiandae sint soluta temporibus tenetur?</p>
                        <p class="chat-content-msg__item--time">10:30 10.09</p>
                      </div>
                       <div class="chat-content-msg__item">
<!--                        avatarVip-->
                        <div class="chat-content-msg__item--img avatarVip">
                           <img  src="https://picsum.photos/400/400?image=73" alt="">
                        </div>

                        <p class="chat-content-msg__item--text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium alias animi deleniti laborum modi mollitia repudiandae sint soluta temporibus tenetur?</p>
                        <p class="chat-content-msg__item--time">10:30 10.09</p>
                      </div>
                      <div class="chat-content-msg__item">
<!--                        avatarVip-->
                        <div class="chat-content-msg__item--img avatarVip">
                           <img  src="https://picsum.photos/400/400?image=73" alt="">
                        </div>

                        <p class="chat-content-msg__item--text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium alias animi deleniti laborum modi mollitia repudiandae sint soluta temporibus tenetur?</p>
                        <p class="chat-content-msg__item--time">10:30 10.09</p>
                      </div>
                       <div class="chat-content-msg__item">
<!--                        avatarVip-->
                        <div class="chat-content-msg__item--img avatarVip">
                           <img  src="https://picsum.photos/400/400?image=73" alt="">
                        </div>

                        <p class="chat-content-msg__item--text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium alias animi deleniti laborum modi mollitia repudiandae sint soluta temporibus tenetur?</p>
                        <p class="chat-content-msg__item--time">10:30 10.09</p>
                      </div>


                    </div>

                    <div class="chat-send-msg">
                      <!--                     <vs-input style="flex-basis: 75%" size="large" placeholder="msg" v-model="value1" />-->
                      <vs-textarea  style="flex-basis: 75%; margin-bottom: 0" label="Yor message"  />
                      <vs-button   color="#28DEEF" type="filled" >
                        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                          <path d="M3 8C3 8.55 3.45 9 4 9C4.55 9 5 8.55 5 8V6H7C7.55 6 8 5.55 8 5C8 4.45 7.55 4 7 4H5V2C5 1.45 4.55 1 4 1C3.45 1 3 1.45 3 2V4H1C0.45 4 0 4.45 0 5C0 5.55 0.45 6 1 6H3V8Z" fill="white"/>
                          <path d="M13 17C14.6569 17 16 15.6569 16 14C16 12.3431 14.6569 11 13 11C11.3431 11 10 12.3431 10 14C10 15.6569 11.3431 17 13 17Z" fill="white"/>
                          <path d="M21 6H17.83L16.59 4.65C16.4036 4.44539 16.1767 4.28191 15.9235 4.16999C15.6704 4.05807 15.3968 4.00017 15.12 4H8.72C8.89 4.3 9 4.63 9 5C9 6.1 8.1 7 7 7H6V8C6 9.1 5.1 10 4 10C3.63 10 3.3 9.89 3 9.72V20C3 21.1 3.9 22 5 22H21C22.1 22 23 21.1 23 20V8C23 6.9 22.1 6 21 6ZM13 19C10.24 19 8 16.76 8 14C8 11.24 10.24 9 13 9C15.76 9 18 11.24 18 14C18 16.76 15.76 19 13 19Z" fill="white"/>
                        </svg>
                      </vs-button>
                      <vs-button   color="#5753E8" type="filled" ><svg width="24" height="24" viewBox="0 0 30 30" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M29.7426 0.257471C29.494 0.00879953 29.121 -0.0676652 28.7947 0.0628814L0.55251 11.3596C0.229366 11.4889 0.0129796 11.7966 0.000557715 12.1445C-0.0118055 12.4923 0.182257 12.8146 0.495381 12.9665L11.6322 18.3677L17.0334 29.5045C17.1807 29.8082 17.4884 29.9999 17.824 29.9999C17.8345 29.9999 17.845 29.9997 17.8555 29.9993C18.2032 29.9869 18.5111 29.7706 18.6403 29.4474L29.9371 1.2054C30.0677 0.878915 29.9912 0.506084 29.7426 0.257471ZM3.05235 12.2529L25.4718 3.28524L12.1108 16.6462L3.05235 12.2529ZM17.747 26.9476L13.3537 17.8891L26.7148 4.52813L17.747 26.9476Z" fill="white"/>
                      </svg>
                      </vs-button>


                    </div>

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
        activeIndex: '2',
      }
    },

  }
</script>


<style>
.el-menu.el-menu--horizontal {
  border-bottom: none;

}
</style>
