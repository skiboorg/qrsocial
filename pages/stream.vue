<template>
  <div>
    <section style="padding-top: 40px">
      <div class="container">
        <div class="girl-profile-stream__wrapper">
          <div class="girl-profile-stream__left">
            <div class="girl-profile-stream-block">
              <div class="girl-profile-stream-block__top">
                <div class="girl-profile-stream-block__top--avatar">
                  <img src="/testw.png" alt="">
                </div>
                <div class="girl-profile-stream-block__top--name">
                  <p>karina kunakuzina</p>
                  <p>@kistochka</p>
                </div>
              </div>
              <div  class="girl-profile-stream-block__content">
                <div v-if="streamBtnActive" @click="cllick1" class="stream-item__top-btn stream-btn-abs">
                  <div class="stream-item__top-btn--inner">
                    <img draggable="false" src="/play_icon.png" alt="">
                  </div>
                </div>
                <video
                  id="my-player"
                  class="video-js vjs-default-skin vjs-big-play-centered">

                  <p class="vjs-no-js">
                    To view this video please enable JavaScript, and consider upgrading to a
                    web browser that
                    <a href="http://videojs.com/html5-video-support/" target="_blank">
                      supports HTML5 video
                    </a>
                  </p>
                </video>

              </div>
              <div class="girl-profile-stream-block__bottom">
                <div class="girl-profile-stream-block__bottom--text">
                  <p>100B</p>
                  <p>Lorem ipsum dolor.</p>
                </div>
                <div @click="giftModal=true" class="girl-profile-stream-block__bottom--btn">
                  <p>选择礼物</p>
                </div>
              </div>
            </div>
          </div>
          <div class="girl-profile-stream__right">
            <div class="chat-content">
              <div class="chat-content__top-donators">
                <div class="chat-content__top-donators--item">
                  <img src="/testw.png" alt="">
                </div>
                <div class="chat-content__top-donators--item vipDonat">
                  <img src="/testw.png" alt="">
                </div>
                <div class="chat-content__top-donators--item">
                  <img src="/testw.png" alt="">
                </div>
              </div>
              <div class="chat-content-msg">
                <div class="chat-content-msg__item">
                  <img class="chat-content-msg__item--img" src="/testw.png" alt="">
                  <p class="chat-content-msg__item--text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium alias animi deleniti laborum modi mollitia repudiandae sint soluta temporibus tenetur?</p>
                  <p class="chat-content-msg__item--time">10:30 10.09</p>
                </div>
                <div class="chat-content-msg__item">
                  <img class="chat-content-msg__item--img" src="/testw.png" alt="">
                  <p class="chat-content-msg__item--text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium alias animi deleniti laborum modi mollitia repudiandae sint soluta temporibus tenetur?</p>
                  <p class="chat-content-msg__item--time">10:30 10.09</p>
                </div>
                <div class="chat-content-msg__item">
                  <img class="chat-content-msg__item--img" src="/testw.png" alt="">
                  <p class="chat-content-msg__item--text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium alias animi deleniti laborum modi mollitia repudiandae sint soluta temporibus tenetur?</p>
                  <p class="chat-content-msg__item--time">10:30 10.09</p>
                </div>
                <div class="chat-content-msg__item ownMsg">
                  <img class="chat-content-msg__item--img" src="/testw.png" alt="">
                  <p class="chat-content-msg__item--text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium alias animi deleniti laborum modi mollitia repudiandae sint soluta temporibus tenetur?</p>
                  <p class="chat-content-msg__item--time">10:30 10.09</p>
                </div>
                <div class="chat-content-msg__item ownMsg">
                  <img class="chat-content-msg__item--img" src="/testw.png" alt="">
                  <p class="chat-content-msg__item--text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium alias animi deleniti laborum modi mollitia repudiandae sint soluta temporibus tenetur?</p>
                  <p class="chat-content-msg__item--time">10:30 10.09</p>
                </div>
                <div class="chat-content-msg__item ">
                  <img class="chat-content-msg__item--img" src="/testw.png" alt="">
                  <p class="chat-content-msg__item--text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium alias animi deleniti laborum modi mollitia repudiandae sint soluta temporibus tenetur?</p>
                  <p class="chat-content-msg__item--time">10:30 10.09</p>
                </div>
              </div>

              <div class="chat-send-msg">
                <!--                     <vs-input style="flex-basis: 75%" size="large" placeholder="msg" v-model="value1" />-->
                <vs-textarea  style="flex-basis: 75%; margin-bottom: 0" label="Yor message"  />

                <vs-button   color="#5753E8" type="filled" ><svg width="24" height="24" viewBox="0 0 30 30" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <path d="M29.7426 0.257471C29.494 0.00879953 29.121 -0.0676652 28.7947 0.0628814L0.55251 11.3596C0.229366 11.4889 0.0129796 11.7966 0.000557715 12.1445C-0.0118055 12.4923 0.182257 12.8146 0.495381 12.9665L11.6322 18.3677L17.0334 29.5045C17.1807 29.8082 17.4884 29.9999 17.824 29.9999C17.8345 29.9999 17.845 29.9997 17.8555 29.9993C18.2032 29.9869 18.5111 29.7706 18.6403 29.4474L29.9371 1.2054C30.0677 0.878915 29.9912 0.506084 29.7426 0.257471ZM3.05235 12.2529L25.4718 3.28524L12.1108 16.6462L3.05235 12.2529ZM17.747 26.9476L13.3537 17.8891L26.7148 4.52813L17.747 26.9476Z" fill="white"/>
                </svg>
                </vs-button>


              </div>

            </div>
          </div>
        </div>
        <vs-popup class="holamundo"  title="Select gift" :active.sync="giftModal">
          <div class="gift-modal__gifts">
            <div class="gift-modal__gift">
              <img src="/g1.png" alt="">
            </div>
            <div class="gift-modal__gift">
              <img src="/g2.png" alt="">
            </div>
            <div class="gift-modal__gift">
              <img src="/g3.png" alt="">
            </div>
            <div class="gift-modal__gift">
              <img src="/g4.png" alt="">
            </div>
            <div class="gift-modal__gift">
              <img src="/g5.png" alt="">
            </div>
            <div class="gift-modal__gift">
              <img src="/g6.png" alt="">
            </div>

          </div>
          <div class="gift-modal__form">
            <vs-select style="margin-right: 20px;flex-basis: 50%;" class="selectExample" v-model="select1" >
              <vs-select-item :key="index" :value="item.value" :text="item.text" v-for="item,index in options1" />
            </vs-select>
             <vs-textarea class="gift-modal__form--text" label="Мessage" v-model="textarea" />
          </div>
          <div >
            <div style="margin: 0 auto" class="btn btn-outline btn-outline-blue">
              <div class="btn-outline-inner">
                <p>女孩</p>
              </div>

            </div>
          </div>
        </vs-popup>
      </div>
    </section>

  </div>
</template>

<script>
  import "video.js/dist/video-js.css";
  import videojs from "video.js";
  import "videojs-flash";
  export default {
    data(){
      return {
        player: null,
        value1:'',
        value2:'',
        value3:'',
        activeTab:'userStreamTab',//'userInfo'
        imageModal:false,
        streamBtnActive:true,
        currentImage:null,
        giftModal:false,
        select1:null,
        textarea:'',
        options1:[
          {text:'IT',value:0},
          {text:'Blade Runner',value:2},
          {text:'Thor Ragnarok',value:3},
        ],
      }
    },

    mounted() {


    },
    methods:{
      showImage(image){
        console.log(image)
      },
      cllick1: function() {
        this.streamBtnActive = false
        var thisp = this;
        let options = {

          height: "360",

          fluid:true,
          playbackRates: [0.5, 1, 1.5, 2, 2.5],
          sources: [
            {
              type: "rtmp/mp4",
              src: "rtmp://95.215.207.100/live/1234"
            }
          ],
          techOrder: ["flash"],
          autoplay: true,
          controls: true,
          poster:
            "http://placehold.it/1920x1080"
        };
        var player = videojs("my-player", options);
        console.log(player);
        player.ready(function() {
          this.play();
        });
        player.on("ended", function() {
          console.log("ended");
        });
        player.on("pause", function() {
          console.log("pause");
        });
        player.on("timeupdate", function() {
          var currentTime = this.currentTime();
          // console.log(thisp.progressLast, currentTime, "视频进度");
          // if (currentTime == thisp.progressLast && currentTime != 0) {
          //   player.pause();
          //   player.load();
          //   player.play();
          //   // player.ready(function() {
          //   //   player.load();
          //   //   player.play();
          //   // });
          // } else {
          //   thisp.progressLast = currentTime;
          // }
        });
        player.on("error", function() {
          console.log("error");
        });
        player.on("waiting", function() {
          console.log("waiting");
        });
        player.on("emptied", function() {
          console.log("emptied");
        });
        this.player = player;
      },
    }
  }
</script>


<style>
  .video-js{
    width: 100% !important;
    height: 400px !important;

  }
  .my-player-dimensions{
    width: 100%;
  }
</style>
