<template>
  <div>
    <section style="padding-top: 40px">
      <div class="container">
         <img class="mb-40" src="/test_streams.png" alt="">
        <div class="streams-wrapper">
          <div class="stream-item ">
            <nuxt-link to="/stream">
              <div class="stream-item__top" style="background: linear-gradient(black, black), url(/test.png) no-repeat center">
                <div class="stream-item__top-btn">
                  <div class="stream-item__top-btn--inner">
                    <img draggable="false" src="/play_icon.png" alt="">
                  </div>
                </div>
                <div class="stream-item__top-for-vip">
                  <img draggable="false" src="/stream_for_vip_icon.png" alt="">
                  <p>只限VIP</p>
                </div>
              </div>
              <div class="stream-item__bottom">
                <div class="stream-item__bottom--left">
                  <p>玛丽的追求</p>
                  <p>4小时前上传</p>
                </div>
                <div class="stream-item__bottom--right">
                  <img draggable="false" src="http://placehold.it/300" alt="">
                </div>
              </div>
            </nuxt-link>
          </div>
          <div class="stream-item ">
            <nuxt-link to="/stream">
              <div class="stream-item__top" style="background: linear-gradient(black, black), url(/test.png) no-repeat center">
                <div class="stream-item__top-btn">
                  <div class="stream-item__top-btn--inner">
                    <img draggable="false" src="/play_icon.png" alt="">
                  </div>
                </div>
                <div class="stream-item__top-for-vip">
                  <img draggable="false" src="/stream_for_vip_icon.png" alt="">
                  <p>只限VIP</p>
                </div>
              </div>
              <div class="stream-item__bottom">
                <div class="stream-item__bottom--left">
                  <p>玛丽的追求</p>
                  <p>4小时前上传</p>
                </div>
                <div class="stream-item__bottom--right">
                  <img draggable="false" src="http://placehold.it/300" alt="">
                </div>
              </div>
            </nuxt-link>
          </div>
          <div class="stream-item stream-vip">
            <nuxt-link to="/stream">
              <div class="stream-item__top" style="background: linear-gradient(black, black), url(/test.png) no-repeat center">
                <div class="stream-item__top-btn">
                  <div class="stream-item__top-btn--inner">
                    <img draggable="false" src="/play_icon.png" alt="">
                  </div>
                </div>
                <div class="stream-item__top-for-vip">
                  <img draggable="false" src="/stream_for_vip_icon.png" alt="">
                  <p>只限VIP</p>
                </div>
              </div>
              <div class="stream-item__bottom">
                <div class="stream-item__bottom--left">
                  <p>玛丽的追求</p>
                  <p>4小时前上传</p>
                </div>
                <div class="stream-item__bottom--right">
                  <img draggable="false" src="http://placehold.it/300" alt="">
                </div>
              </div>
            </nuxt-link>
          </div>
          <div class="stream-item stream-vip">
            <nuxt-link to="/stream">
              <div class="stream-item__top" style="background: linear-gradient(black, black), url(/test.png) no-repeat center">
                <div class="stream-item__top-btn">
                  <div class="stream-item__top-btn--inner">
                    <img draggable="false" src="/play_icon.png" alt="">
                  </div>
                </div>
                <div class="stream-item__top-for-vip">
                  <img draggable="false" src="/stream_for_vip_icon.png" alt="">
                  <p>只限VIP</p>
                </div>
              </div>
              <div class="stream-item__bottom">
                <div class="stream-item__bottom--left">
                  <p>玛丽的追求</p>
                  <p>4小时前上传</p>
                </div>
                <div class="stream-item__bottom--right">
                  <img draggable="false" src="http://placehold.it/300" alt="">
                </div>
              </div>
            </nuxt-link>
          </div>
        </div>
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
        currentImage:null,
      }
    },

  }
</script>


<style>

</style>
