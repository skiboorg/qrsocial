<template>
  <div>
    <section class="girl-login-page">



      <vs-card  class="cardx girl-login">
      <div class="girl-login__header" slot="header"><p>вход для девушек</p> </div>

        <div>
           <vs-input label-placeholder="Label-placeholder" v-model="value1"/>
           <vs-input label-placeholder="Label-placeholder" v-model="value2"/>
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
