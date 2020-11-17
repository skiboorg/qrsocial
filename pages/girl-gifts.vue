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
<div class="block-rounded p50">
      <vs-table class="mb-40" :data="users">



          <template slot-scope="{data}">
            <vs-tr :key="indextr" v-for="(tr, indextr) in data" >

              <vs-td :data="data[indextr].img">
                <div :class="{'avatarVip':data[indextr].vip}">
                  <img  style="width: 40px;height: 40px;border-radius: 100%; object-fit: cover" :src="data[indextr].img" alt="">
                </div>
              </vs-td>
              <vs-td :data="data[indextr].gift">

                  <img  style="width: 40px;height: 40px;border-radius: 100%; object-fit: cover" :src="data[indextr].gift" alt="">

              </vs-td>
              <vs-td :data="data[indextr].rating">
                {{data[indextr].amount}}
              </vs-td>

              <vs-td :data="data[indextr].name">
                {{data[indextr].name}}
              </vs-td>

              <vs-td :data="data[indextr].login">
                {{data[indextr].login}}
              </vs-td>
               <vs-td :data="data[indextr].message">
                {{data[indextr].message}}
              </vs-td>
               <vs-td >
                 <div class="btn btn-l-blue-solid btn-hover-shadow"><p>Написать сообщение</p></div>

              </vs-td>


            </vs-tr>
          </template>
        </vs-table>
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
        activeIndex: '5',
         users:[
          {
            "id": 1,
            "img":'https://media.gettyimages.com/photos/teenage-beauty-picture-id1126913832?s=2048x2048',
            "vip":true,
            "amount": "+ 90b",
            "name": "CHI HUANG",
            "login": "@YGYGY2",
            'gift':'/gift1.png',
            "message":'ты самая красивая на свете'
          },
          {
            "id": 2,
            "img":'https://images.unsplash.com/photo-1529626455594-4ff0802cfb7e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=634&q=80',
            "amount": "+ 90b",
            "vip":false,
            "name": "CHI HUANG",
            "login": "@YGYGY2",
            'gift':'/gift2.png',
            "message":'ты самая красивая на свете'
          },
          {
            "id": 3,
            "img":'https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=634&q=80',
            "vip":false,
            "amount": "+ 90b",
            "name": "CHI HUANG",
            "login": "@YGYGY2",
            'gift':'/gift3.png',
            "message":'ты самая красивая на свете'
          },
             {
            "id": 4,
            "img":'https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=634&q=80',
            "vip":false,
            "amount": "+ 90b",
            "name": "CHI HUANG",
            "login": "@YGYGY2",
            'gift':'/gift1.png',
            "message":'ты самая красивая на свете'
          },
             {
            "id": 5,
            "img":'https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=634&q=80',
            "vip":false,
            "amount": "+ 90b",
            "name": "CHI HUANG",
            "login": "@YGYGY2",
            'gift':'/gift4.png',
            "message":'ты самая красивая на свете'
          },
             {
            "id": 6,
            "img":'https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=634&q=80',
            "vip":false,
            "amount": "+ 90b",
            "name": "CHI HUANG",
            "login": "@YGYGY2",
            'gift':'/gift5.png',
            "message":'ты самая красивая на свете'
          },



        ]
      }
    },

  }
</script>


<style>
.el-menu.el-menu--horizontal {
  border-bottom: none;

}
</style>
