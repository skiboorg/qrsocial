<template>
  <div>
    <section class="girl-login-page">



      <vs-card  class="cardx girl-login">
      <div class="girl-login__header" slot="header"><p>вход для девушек</p> </div>

        <div style="padding: 20px 60px">
           <vs-input style="width: 100%;margin-bottom: 30px"  size="large" label-placeholder="ваша почта" v-model="value1"/>
           <vs-input style="width: 100%;margin-bottom: 10px"  size="large" label-placeholder="ваш телефон" v-model="value2"/>
          <p style="text-align: end;margin-bottom: 20px">ЗАБЫЛИ ПАРОЛЬ?</p>


          <nuxt-link to="/girl-lk"><vs-button style="width: 100%;margin-bottom: 10px" color="success" type="gradient">войти в личный кабинет</vs-button></nuxt-link>
          <nuxt-link to="/girl-login-s1"> <vs-button style="width: 100%;margin-bottom: 10px" color="danger" type="gradient">зарегистрироваться</vs-button></nuxt-link>

        </div>

      </vs-card>

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

</style>
