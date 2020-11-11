<template>
  <div>
    <section class="girl-login-page">
      <div class="container entrance-top">
        <img src="/e1.png" alt="">
      <img src="/e2.png" alt="">
      </div>
      <div class="entrance-form">
        <vs-tabs>
      <vs-tab label="登录到您的个人帐户">
        <div class="con-tab-ejemplo">
            <vs-card  class="cardx girl-login">


        <div >
           <vs-input style="width: 100%;margin-bottom: 10px"  size="large" label-placeholder="输入您的登录名" v-model="value1"/>
           <vs-input style="width: 100%;margin-bottom: 50px"  size="large" label-placeholder="输入密码" v-model="value2"/>


        <div style="display: flex; align-items: center;justify-content: space-between" class="">
          <nuxt-link style="color: #FFFFff; margin-right: 20px" to="/girl-lk"><div style="padding: 10px; width: 230px" class="btn btn-l-blue-solid">输入您的个人帐户</div></nuxt-link>
          <nuxt-link to="/girl-login-s1">  <div style=" width: 230px" class="btn btn-outline btn-outline-d-blue">
                  <div  style="padding: 10px" class="btn-outline-inner">
                    <p>
                      忘记密码或无法访问？
                    </p>
                  </div>
                </div></nuxt-link>
        </div>


        </div>

      </vs-card>
        </div>
      </vs-tab>
      <vs-tab label="在我们的门户网站上注册">
        <div class="con-tab-ejemplo">
              <vs-card  class="cardx girl-login">


        <div >
           <vs-input style="width: 100%;margin-bottom: 10px"  size="large" label-placeholder="输入您的登录名" v-model="value1"/>
           <vs-input style="width: 100%;margin-bottom: 50px"  size="large" label-placeholder="输入密码" v-model="value2"/>


        <div style="display: flex; align-items: center;justify-content: space-between" class="">
          <nuxt-link style="color: #FFFFff; margin-right: 20px" to="/girl-lk"><div style="padding: 10px; width: 230px" class="btn btn-l-blue-solid">输入您的个人帐户</div></nuxt-link>
          <nuxt-link to="/girl-login-s1">  <div style=" width: 230px" class="btn btn-outline btn-outline-d-blue">
                  <div  style="padding: 10px" class="btn-outline-inner">
                    <p>
                      忘记密码或无法访问？
                    </p>
                  </div>
                </div></nuxt-link>
        </div>


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
