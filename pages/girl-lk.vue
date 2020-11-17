<template>
  <div>

  <div class="girl-lk-header">
    <el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" >
  <el-menu-item index="1"><nuxt-link to="/girl-lk">МОЙ ПРОФИЛЬ</nuxt-link></el-menu-item>
  <el-menu-item index="2"><nuxt-link to="/girl-lk-chat">МОИ ЧАТЫ</nuxt-link></el-menu-item>
  <el-menu-item index="3"><nuxt-link to="/girl-lk-streams">МОИ ТРАНСЛЯЦИИ</nuxt-link></el-menu-item>
  <el-menu-item index="4"><nuxt-link to="/girl-lk">МОИ ДРУЗЬЯ</nuxt-link></el-menu-item>
      <el-menu-item index="5"><nuxt-link to="/girl-gifts">МОИ Подарки</nuxt-link></el-menu-item>

</el-menu>
<div class="line"></div>
    <div class="girl-lk-header__right">
      <el-tag style="margin-right: 20px" effect="plain" type="info">5000 B</el-tag>
       <el-button icon="el-icon-bell" circle></el-button>
       <el-button icon="el-icon-chat-line-round" circle></el-button>
    </div>
  </div>
<div class="container">
   <p class="section-subheader  mb-40">МОИ ДАННЫЕ</p>
     <div class="block-rounded p50">

                  <div style="display: flex;align-items: center;justify-content: flex-start">
                     <vs-upload style="margin-right: 20px" action="https://jsonplaceholder.typicode.com/posts/" text="Change avatar" :show-upload-button="false" @on-success="successUpload" />
                   <vs-upload action="https://jsonplaceholder.typicode.com/posts/" text="Change BG" :show-upload-button="false" @on-success="successUpload" />
                  </div>
                  <div class="profile-user-info__form">
                  <div class="">
                    <vs-input style="width: 100%" size="default" label-placeholder="логин" v-model="value1"/>
                    <vs-input style="width: 100%" label-placeholder="пароль" v-model="value2"/>
                    <vs-input style="width: 100%" size="default" label-placeholder="почта" v-model="value1"/>

                  </div>
                   <div class="">
                    <vs-input style="width: 100%" size="default" label-placeholder="логин" v-model="value1"/>
                    <vs-input style="width: 100%" label-placeholder="пароль" v-model="value2"/>
                    <vs-input style="width: 100%" size="default" label-placeholder="почта" v-model="value1"/>

                  </div>
                </div>
               <vs-button style="width: 300px" color="success" type="gradient">Сохранить</vs-button>
              </div>
  <p class="section-subheader  mb-40">МОИ ФОТОГРАФИИ</p>
  <div class="mb-40"> <vs-button style="width: 300px" color="warning" type="gradient">добавить альбом</vs-button>
    <vs-button style="width: 300px" color="success" type="gradient">добавить фото</vs-button></div>

  <div class="girl-profile-albums">
            <div class="girl-profile-album" style="background:linear-gradient(black, black), url(https://media.gettyimages.com/photos/young-beautiful-woman-picture-id1050903354?s=2048x2048) no-repeat center">
              <div class="girl-profile-album__counter">
                <p>47</p></div>
              <div class="girl-profile-album__title">个人资料照片</div>
              <div class="girl-profile-album__subtitle">1周前更新</div>
            </div>
            <div class="girl-profile-album  " style="background:linear-gradient(black, black), url(https://media.gettyimages.com/photos/young-beautiful-woman-picture-id1050903354?s=2048x2048) no-repeat center">
              <div class="girl-profile-album__locked">
                <img src="/stream_for_vip_icon.png" alt="">
              </div>
              <div class="girl-profile-album__counter">
                <p>47</p></div>
              <div class="girl-profile-album__title">个人资料照片</div>
              <div class="girl-profile-album__subtitle">1周前更新</div>
            </div>
            <div class="girl-profile-album" style="background: url(https://media.gettyimages.com/photos/young-beautiful-woman-picture-id1050903354?s=2048x2048) no-repeat center">
              <div class="girl-profile-album__counter">
                <p>47</p></div>
              <div class="girl-profile-album__title">个人资料照片</div>
              <div class="girl-profile-album__subtitle">1周前更新</div>
            </div>
            <div class="girl-profile-album" style="background: url(https://media.gettyimages.com/photos/young-beautiful-woman-picture-id1050903354?s=2048x2048) no-repeat center">
              <div class="girl-profile-album__counter">
                <p>47</p></div>
              <div class="girl-profile-album__title">个人资料照片</div>
              <div class="girl-profile-album__subtitle">1周前更新</div>
            </div>
          </div>


          <p class="section-subheader mb-50">альбом 1</p>
          <div class="girl-profile-album-content">
            <div @click="currentImage='https://media.gettyimages.com/photos/young-beautiful-woman-picture-id1050903354?s=2048x2048',imageModal=true" class="girl-profile-album-content__item">
              <img src="https://media.gettyimages.com/photos/young-beautiful-woman-picture-id1050903354?s=2048x2048" alt="">
            </div>
            <div @click="currentImage='https://media.gettyimages.com/photos/young-beautiful-woman-picture-id1050903354?s=2048x2048',imageModal=true" class="girl-profile-album-content__item">
              <img src="https://media.gettyimages.com/photos/young-beautiful-woman-picture-id1050903354?s=2048x2048" alt="">
            </div>
            <div @click="currentImage='https://media.gettyimages.com/photos/young-beautiful-woman-picture-id1050903354?s=2048x2048',imageModal=true" class="girl-profile-album-content__item">
              <img src="https://media.gettyimages.com/photos/young-beautiful-woman-picture-id1050903354?s=2048x2048" alt="">
            </div>
            <div @click="currentImage='https://media.gettyimages.com/photos/young-beautiful-woman-picture-id1050903354?s=2048x2048',imageModal=true" class="girl-profile-album-content__item">
              <img src="https://media.gettyimages.com/photos/young-beautiful-woman-picture-id1050903354?s=2048x2048" alt="">
            </div>
            <div @click="currentImage='https://media.gettyimages.com/photos/young-beautiful-woman-picture-id1050903354?s=2048x2048',imageModal=true" class="girl-profile-album-content__item">
              <img src="https://media.gettyimages.com/photos/young-beautiful-woman-picture-id1050903354?s=2048x2048" alt="">
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
        activeIndex: '1',
      }
    },

  }
</script>


<style>
.el-menu.el-menu--horizontal {
  border-bottom: none;

}
</style>
