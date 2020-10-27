<template>
  <div class="group-item">
            <div class="group-item__top" style="background: url(http://placehold.it/400x100)"></div>
            <div class="group-item__button">
              <img draggable="false" src="/group_icon.png" alt="">
            </div>
            <div class="group-item__img">
              <img draggable="false" src="http://placehold.it/100" alt="">
            </div>
            <div class="group-item__title">{{title}}</div>
            <div class="group-item__subtitle">{{subtitle}}</div>
            <div class="group-item__numbers">
              <div class="group-item__number">
                <p>120</p>
                <p>广播的数</p>
              </div>
              <div class="group-item__number">
                <p>120</p>
                <p>广播的数</p>
              </div>
              <div class="group-item__number">
                <p>120</p>
                <p>广播的数</p>
              </div>
            </div>
            <div class="group-item__avatars">
              <span class="group-item__avatar">
                  <img src="https://www.fillmurray.com/50/50" width="50" height="50"/>
              </span>
              <span class="group-item__avatar">
                  <img src="https://www.fillmurray.com/100/100" width="50" height="50"/>
              </span>
              <span class="group-item__avatar">
                <img src="https://www.fillmurray.com/200/200" width="50" height="50"/>
              </span>
              <span class="group-item__avatar">
                <img src="https://www.fillmurray.com/150/150" width="50" height="50"/>
              </span>
              <span class="group-item__avatar">
                  <img src="https://www.fillmurray.com/50/50" width="50" height="50"/>
              </span>
              <span class="group-item__avatar">
                  <p>+ 12</p>
              </span>
            </div>
            <div class="btn btn-blue-solid"><p>加入小组</p></div>

          </div>
</template>

<script>
  export default {
    props:['title','subtitle',],

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


