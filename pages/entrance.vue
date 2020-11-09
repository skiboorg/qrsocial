<template>
  <div>
    <section class="girl-login-page">
      <div class="container entrance-top">
        <img src="http://placehold.it/590x190" alt="">
      <img src="http://placehold.it/590x190" alt="">
      </div>
      <div class="entrance-form">
        <vs-tabs>
      <vs-tab label="Вход">
        <div class="con-tab-ejemplo">
            <vs-card  class="cardx girl-login">


        <div style="padding: 20px 60px">
           <vs-input style="width: 100%;margin-bottom: 30px"  size="large" label-placeholder="ваша почта" v-model="value1"/>
           <vs-input style="width: 100%;margin-bottom: 10px"  size="large" label-placeholder="ваш телефон" v-model="value2"/>
          <p style="text-align: end;margin-bottom: 20px">ЗАБЫЛИ ПАРОЛЬ?</p>


          <nuxt-link to="/girl-lk"><vs-button style="width: 100%;margin-bottom: 10px" color="success" type="gradient">войти в личный кабинет</vs-button></nuxt-link>
          <nuxt-link to="/girl-login-s1"> <vs-button style="width: 100%;margin-bottom: 10px" color="danger" type="gradient">зарегистрироваться</vs-button></nuxt-link>

        </div>

      </vs-card>
        </div>
      </vs-tab>
      <vs-tab label="Регистрация">
        <div class="con-tab-ejemplo">
           <vs-card  class="cardx girl-login">


        <div style="padding: 20px 60px">
           <vs-input style="width: 100%;margin-bottom: 30px"  size="large" label-placeholder="ваша почта" v-model="value1"/>
           <vs-input style="width: 100%;margin-bottom: 10px"  size="large" label-placeholder="ваш телефон" v-model="value2"/>
          <p style="text-align: end;margin-bottom: 20px">ЗАБЫЛИ ПАРОЛЬ?</p>


          <nuxt-link to="/girl-lk"><vs-button style="width: 100%;margin-bottom: 10px" color="success" type="gradient">войти в личный кабинет</vs-button></nuxt-link>
          <nuxt-link to="/girl-login-s1"> <vs-button style="width: 100%;margin-bottom: 10px" color="danger" type="gradient">зарегистрироваться</vs-button></nuxt-link>

        </div>

      </vs-card>
        </div>
      </vs-tab>

    </vs-tabs>
      </div>






    </section>

  </div>
</template>

<script>

  export default {
    layout: 'login',
    data(){
      return {
        value1:'',
        value2:'',
      }
    },

  }
</script>


<style>
.con-vs-tabs{
  width: unset;
}
  .vs-tabs--li{
    width: 50%;
  }
.vs-tabs--ul{
 box-shadow: none;
}
  .vs-tabs--content{
    padding: 40px;

  }
.con-vs-card{
  box-shadow: none;
}
</style>
