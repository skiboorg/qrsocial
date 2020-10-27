<template>
  <div>
    <section class="girl-profile">
      <div class="container">
        <div class="girl-profile-area">
          <div class="girl-profile-area__img" style="background: url(/test_p_g_bg.png) no-repeat center"></div>
          <div class="girl-profile-area__avatar">
            <img src="https://picsum.photos/400/400?image=200" alt="">
          </div>
          <div class="girl-profile-area__info">
            <div class="girl-profile-area__info--top">
              <div class="girl-profile-area__info--stats">
                <div class="girl-profile-area__info--stats--item">
                  <img src="/g-profile-stat-icon1.png" alt="">
                  <div class="">
                    <p>7124</p>
                    <p>广播评级</p>
                  </div>
                </div>
                <div class="girl-profile-area__info--stats--item">
                  <img src="/g-profile-stat-icon1.png" alt="">
                  <div class="">
                    <p>7124</p>
                    <p>广播评级</p>
                  </div>
                </div>
                <div class="girl-profile-area__info--stats--item">
                  <img src="/g-profile-stat-icon1.png" alt="">
                  <div class="">
                    <p>7124</p>
                    <p>广播评级</p>
                  </div>
                </div>
              </div>
              <div class="girl-profile-area__info--buttons">
                <div class="btn btn-blue btn-round"><p>text</p></div>
                <div class="btn btn-blue btn-round"><p>text</p></div>
              </div>
            </div>
            <div class="girl-profile-area__info--bottom">
              <p>dsfdsf</p>
              <p>sdfdsf</p>
            </div>

          </div>

        </div>
        <div class="girl-profile-menu">
          <div class="girl-profile-menu__item " @click="activeTab='userInfo'" :class="{'girlMenuItemActive':activeTab==='userInfo'}">
            <svg class="girl-profile-menu__item--img" width="40" height="40" viewBox="0 0 40 40" fill="none" xmlns="http://www.w3.org/2000/svg">
              <g clip-path="url(#clip0)">
                <path d="M36.8424 40.0003H32.7893C32.7893 33.1628 27.0542 27.6019 19.9998 27.6019C12.9454 27.6019 7.21227 33.1648 7.21227 40.0003H3.15918C3.15918 30.9255 10.7162 23.5488 20.0018 23.5488C29.2854 23.5488 36.8424 30.9255 36.8424 40.0003Z" />
                <path d="M20.0013 22.2312C13.875 22.2312 8.8877 17.2419 8.8877 11.1156C8.88567 4.98733 13.873 0 20.0013 0C26.1316 0 31.1189 4.98531 31.1189 11.1156C31.1189 17.2459 26.1316 22.2312 20.0013 22.2312ZM20.0013 4.0531C16.1063 4.0531 12.9388 7.22059 12.9388 11.1156C12.9388 15.0106 16.1063 18.1781 20.0013 18.1781C23.8983 18.1781 27.0658 15.0106 27.0658 11.1156C27.0658 7.22059 23.8943 4.0531 20.0013 4.0531Z" />
              </g>
              <defs>
                <clipPath id="clip0">
                  <rect width="40" height="40" fill="white"/>
                </clipPath>
              </defs>
            </svg>
            <p class="girl-profile-menu__item--text">关于我</p>
          </div>
          <div class="girl-profile-menu__item " @click="activeTab='userFriends'" :class="{'girlMenuItemActive':activeTab==='userFriends'}">
            <svg class="girl-profile-menu__item--img" width="77" height="40" viewBox="0 0 77 40" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M26.5098 35.2499H26.5598V35.1999C26.5598 28.2745 20.8132 22.6468 13.7557 22.6468C6.6966 22.6468 0.95 28.2745 0.95 35.1999V35.2499H1H4.06959H4.11959V35.1999C4.11959 30.0338 8.43786 25.8271 13.7542 25.8271C19.0705 25.8271 23.3903 30.0323 23.3903 35.1999V35.2499H23.4403H26.5098Z"   stroke-width="0.1"/>
              <path d="M5.28789 13.2477C5.2879 17.9311 9.08724 21.7456 13.7547 21.7456C18.4252 21.7456 22.2246 17.9342 22.2246 13.2477C22.2246 8.56118 18.4252 4.7498 13.7547 4.7498C9.08572 4.7498 5.28636 8.56273 5.28789 13.2477V13.2477ZM8.45595 13.2477C8.45595 10.3149 10.8326 7.93016 13.7547 7.93016C16.6753 7.93016 19.055 10.3149 19.055 13.2477C19.055 16.1805 16.6784 18.5652 13.7547 18.5652C10.8326 18.5652 8.45595 16.1805 8.45595 13.2477Z"   stroke-width="0.1"/>
              <path d="M76.0006 35.2499H76.0506V35.1999C76.0506 28.2757 70.4559 22.6468 63.5821 22.6468C56.7068 22.6468 51.1121 28.2757 51.1121 35.1999V35.2499H51.1621H54.1509H54.2009V35.1999C54.2009 30.0326 58.4062 25.8271 63.5806 25.8271C68.7551 25.8271 72.9618 30.031 72.9618 35.1999V35.2499H73.0118H76.0006Z"   stroke-width="0.1"/>
              <path d="M63.583 21.7456C59.0364 21.7456 55.3377 17.9298 55.3377 13.2477L63.583 21.7456ZM63.583 21.7456C68.1326 21.7456 71.8313 17.9329 71.8313 13.2477C71.8313 8.56245 68.1326 4.7498 63.583 4.7498C59.0349 4.7498 55.3362 8.564 55.3377 13.2477L63.583 21.7456ZM58.425 13.2477C58.425 10.3136 60.7398 7.93016 63.583 7.93016C66.4248 7.93016 68.7425 10.3137 68.7425 13.2477C68.7425 16.1817 66.4278 18.5652 63.583 18.5652C60.7398 18.5652 58.425 16.1817 58.425 13.2477Z"   stroke-width="0.1"/>
              <path d="M55.2531 40.0004H51.2141C51.2141 33.1628 45.499 27.6019 38.4693 27.6019C31.4395 27.6019 25.7264 33.1648 25.7264 40.0004H21.6875C21.6875 30.9255 29.2181 23.5488 38.4713 23.5488C47.7225 23.5488 55.2531 30.9255 55.2531 40.0004Z" />
              <path d="M38.4703 22.2313C32.3654 22.2313 27.3955 17.2419 27.3955 11.1156C27.3935 4.98734 32.3634 0 38.4703 0C44.5792 0 49.5491 4.98532 49.5491 11.1156C49.5491 17.2459 44.5792 22.2313 38.4703 22.2313ZM38.4703 4.0531C34.5889 4.0531 31.4324 7.2206 31.4324 11.1156C31.4324 15.0107 34.5889 18.1782 38.4703 18.1782C42.3537 18.1782 45.5101 15.0107 45.5101 11.1156C45.5101 7.2206 42.3497 4.0531 38.4703 4.0531Z" />
            </svg>
            <p class="girl-profile-menu__item--text">团体</p>
          </div>
          <div class="girl-profile-menu__item " @click="activeTab='userGallery'" :class="{'girlMenuItemActive':activeTab==='userGallery'}">
            <svg class="girl-profile-menu__item--img" width="47" height="42" viewBox="0 0 47 42" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M23.7895 14.8682C21.113 14.8682 18.9492 17.0677 18.9492 19.7735C18.9492 22.4793 21.1129 24.6789 23.7895 24.6789C26.4659 24.6789 28.6297 22.4794 28.6297 19.7735C28.6297 17.0677 26.466 14.8682 23.7895 14.8682ZM23.7895 21.962C22.6029 21.962 21.635 20.9855 21.635 19.7734C21.635 18.5614 22.6029 17.5849 23.7895 17.5849C24.976 17.5849 25.9439 18.5614 25.9439 19.7734C25.9439 20.9855 24.976 21.962 23.7895 21.962Z"  stroke-width="0.5"/>
              <path d="M42.1236 4.22903L42.1249 4.22918C44.6702 4.53558 46.4936 6.85918 46.2235 9.43601L46.2233 9.4377L43.7096 31.9385L43.7095 31.9389C43.57 33.1673 42.9727 34.296 42.0387 35.0935L42.0298 35.1011L42.0202 35.1079C41.4243 35.5268 40.7556 35.8267 40.0499 35.992V36.6768C40.0499 39.2736 37.731 41.2496 35.2096 41.2496H5.21085C5.15302 41.2504 5.09492 41.25 5.03675 41.2485C5.03674 41.2485 5.03673 41.2485 5.03672 41.2485L5.04345 40.9986C2.75051 40.9371 0.940916 39.0022 1.00148 36.6768L42.1236 4.22903ZM42.1236 4.22903L12.2906 0.793444C11.0637 0.61759 9.82151 0.980638 8.87573 1.79039C7.93231 2.53415 7.32832 3.63425 7.20133 4.83742L6.68161 9.15994H5.20923C2.6399 9.15994 0.751477 11.4617 0.751477 14.0098V36.6736L42.1236 4.22903ZM37.3641 36.4268H37.364V36.6768C37.364 37.7164 36.3194 38.5328 35.2096 38.5328H5.20923V38.5327L5.20179 38.5329C4.25718 38.561 3.463 37.8065 3.435 36.8398L3.435 36.8397C3.43353 36.79 3.43417 36.7403 3.43692 36.6906L3.4373 36.6906V36.6768V32.7011L11.8069 26.4582L11.8069 26.4582L11.811 26.455C12.7308 25.7388 14.0256 25.8022 14.8735 26.6055L14.8734 26.6056L14.8789 26.6104L20.8353 31.9308L20.8352 31.9309L20.8397 31.9347C21.7882 32.7423 22.9827 33.1942 24.2221 33.2136L24.2229 33.2136C25.1927 33.2256 26.1463 32.9639 26.9773 32.4577C26.9779 32.4573 26.9785 32.457 26.9791 32.4566L37.3641 26.3618V36.4268ZM37.364 14.018V23.1778L25.5741 30.1436L25.5725 30.1446C24.643 30.7031 23.4669 30.6027 22.642 29.8939L16.6328 24.5196L16.6328 24.5196L16.6304 24.5175C14.8191 22.939 12.1706 22.8417 10.2514 24.2836C10.251 24.2839 10.2506 24.2841 10.2503 24.2844L3.4373 29.3096V14.0098C3.4373 12.8741 4.19396 11.8768 5.20923 11.8768H35.2042C36.3532 11.9277 37.2858 12.8472 37.364 14.018ZM43.5405 9.10428L43.5405 9.1044L40.9722 31.6052L40.9705 31.6202L40.9706 31.6354C40.9744 32.1428 40.7462 32.6223 40.3544 32.9343L40.3427 32.9436L40.3321 32.9543C40.2735 33.0138 40.1738 33.0687 40.0498 33.128V14.0098H40.0499L40.0496 14.0013C39.9589 11.3471 37.8411 9.22029 35.2152 9.16001L35.2152 9.15994H35.2095H9.36913L9.8282 5.12495C9.92504 4.62743 10.1809 4.17697 10.5555 3.84294C10.9837 3.54659 11.4988 3.40859 12.015 3.45153L41.7928 6.94252L41.7928 6.94257L41.7979 6.94307C42.8591 7.04528 43.6438 8.0025 43.5422 9.08739L43.5405 9.10428Z"  stroke-width="0.5"/>
            </svg>
            <p class="girl-profile-menu__item--text">相片</p>
          </div>
          <div class="girl-profile-menu__item " @click="activeTab='userStreamTab'" :class="{'girlMenuItemActive':activeTab==='userStreamTab'}">
            <svg class="girl-profile-menu__item--img" width="40" height="40" viewBox="0 0 40 40" fill="none" xmlns="http://www.w3.org/2000/svg">
              <g clip-path="url(#clip0)">
                <path d="M35.4285 18.6924H4.53827C2.38037 18.6924 0.625 20.4478 0.625 22.6057V36.0871C0.625 38.2447 2.38037 40.0001 4.53827 40.0001H35.4285C37.5864 40.0001 39.3417 38.2447 39.3417 36.0871V22.6057C39.3417 20.4478 37.5864 18.6924 35.4285 18.6924ZM36.998 36.0871C36.998 36.9523 36.2939 37.6563 35.4285 37.6563H4.53827C3.67279 37.6563 2.96875 36.9523 2.96875 36.0871V22.6057C2.96875 21.7402 3.67279 21.0361 4.53827 21.0361H35.4285C36.2939 21.0361 36.998 21.7402 36.998 22.6057V36.0871Z" />
                <path d="M19.987 12.5498C20.9181 12.5498 21.8492 12.1962 22.5581 11.4884C23.2457 10.8024 23.6241 9.88994 23.6241 8.91917C23.6241 7.94841 23.2457 7.03593 22.5581 6.3499C21.1403 4.9348 18.8334 4.9348 17.4156 6.3499C16.728 7.03593 16.3496 7.94841 16.3496 8.91917C16.3496 9.88994 16.728 10.8024 17.4156 11.4884C18.1245 12.1962 19.0556 12.5498 19.987 12.5498ZM19.0712 8.00853C19.3239 7.75645 19.6553 7.63072 19.987 7.63072C20.3184 7.63072 20.6498 7.75676 20.9022 8.00853C21.1461 8.25175 21.2803 8.57524 21.2803 8.91917C21.2803 9.26311 21.1461 9.58629 20.9025 9.82982C20.3975 10.3337 19.5762 10.3334 19.0712 9.82982C18.8273 9.58629 18.6934 9.26311 18.6934 8.91917C18.6934 8.57524 18.8276 8.25206 19.0712 8.00853Z" />
                <path d="M24.2681 14.044C24.497 14.2735 24.7973 14.3882 25.0975 14.3882C25.3972 14.3882 25.6966 14.2741 25.9255 14.0458C27.2973 12.6765 28.0529 10.8561 28.0529 8.91947C28.0529 6.98283 27.2973 5.16215 25.9255 3.79313C25.4674 3.33598 24.7252 3.33659 24.2681 3.79466C23.8109 4.25272 23.8118 4.99491 24.2699 5.45206C25.1979 6.37827 25.7091 7.60966 25.7091 8.91947C25.7091 10.229 25.1979 11.4607 24.2699 12.3869C23.8118 12.844 23.8109 13.5859 24.2681 14.044Z" />
                <path d="M14.0405 14.0456C14.2693 14.2739 14.5687 14.388 14.8684 14.388C15.1687 14.388 15.469 14.2733 15.6979 14.0438C16.155 13.5857 16.1541 12.8438 15.696 12.3867C14.768 11.4601 14.2568 10.2288 14.2568 8.91895C14.2568 7.60944 14.768 6.37805 15.696 5.45154C16.1541 4.99439 16.155 4.2525 15.6979 3.79443C15.2407 3.33606 14.4985 3.33545 14.0405 3.7926C12.6687 5.16193 11.9134 6.9823 11.9131 8.91895C11.9131 10.8556 12.6687 12.6763 14.0405 14.0456Z" />
                <path d="M10.8118 32.9671H7.66602V24.5537C7.66602 23.9064 7.14142 23.3818 6.49414 23.3818C5.84686 23.3818 5.32227 23.9064 5.32227 24.5537V34.139C5.32227 34.7863 5.84686 35.3109 6.49414 35.3109H10.8118C11.4587 35.3109 11.9836 34.7863 11.9836 34.139C11.9836 33.492 11.4587 32.9671 10.8118 32.9671Z" />
                <path d="M14.4424 23.3818C13.7951 23.3818 13.2705 23.9064 13.2705 24.5537V34.139C13.2705 34.7863 13.7951 35.3109 14.4424 35.3109C15.0894 35.3109 15.6143 34.7863 15.6143 34.139V24.5537C15.6143 23.9064 15.0894 23.3818 14.4424 23.3818Z" />
                <path d="M24.6911 23.4317C24.0719 23.2446 23.4176 23.5953 23.2306 24.2148L21.4587 30.0842L19.6866 24.2148C19.4995 23.595 18.8455 23.2446 18.226 23.4317C17.6065 23.6188 17.2558 24.2728 17.4429 24.8923L20.3369 34.4775C20.3372 34.4784 20.3375 34.4794 20.3378 34.4803C20.6567 35.5008 22.2278 35.5627 22.5796 34.4803C22.5799 34.4794 22.5802 34.4787 22.5805 34.4775L25.4745 24.8923C25.6616 24.2725 25.3106 23.6188 24.6911 23.4317Z" />
                <path d="M33.4721 25.7256C34.1194 25.7256 34.644 25.201 34.644 24.5537C34.644 23.9064 34.1194 23.3818 33.4721 23.3818H28.1855C27.5383 23.3818 27.0137 23.9064 27.0137 24.5537V34.139C27.0137 34.7863 27.5383 35.3109 28.1855 35.3109H33.3143C33.9616 35.3109 34.4862 34.7863 34.4862 34.139C34.4862 33.492 33.9616 32.9671 33.3143 32.9671H29.3574V29.9147H32.6829C33.3302 29.9147 33.8548 29.3901 33.8548 28.7429C33.8548 28.0956 33.3302 27.571 32.6829 27.571H29.3574V25.7256H33.4721Z" />
                <path d="M29.7914 8.91959C29.7914 11.5325 28.7718 13.9895 26.9203 15.8373C26.4622 16.2945 26.4613 17.0367 26.9185 17.4947C27.1477 17.7239 27.4476 17.8387 27.7479 17.8387C28.0476 17.8387 28.347 17.7245 28.5759 17.4963C30.8711 15.2056 32.1351 12.1596 32.1351 8.91959C32.1351 5.67985 30.8711 2.63358 28.5759 0.342934C28.1178 -0.114219 27.3759 -0.113609 26.9185 0.34446C26.4613 0.802529 26.4622 1.54472 26.9203 2.00187C28.7718 3.84971 29.7914 6.30637 29.7914 8.91959Z" />
                <path d="M12.2183 17.8384C12.5186 17.8384 12.8189 17.7237 13.0477 17.4945C13.5049 17.0364 13.5043 16.2943 13.0459 15.8371C11.1944 13.9893 10.1748 11.5323 10.1748 8.91907C10.1748 6.30615 11.1944 3.84918 13.0459 2.00134C13.504 1.54419 13.5049 0.802003 13.0477 0.344239C12.5903 -0.114135 11.8484 -0.114745 11.3903 0.342408C9.09509 2.63336 7.83105 5.67932 7.83105 8.91907C7.83105 12.1591 9.09509 15.2051 11.3903 17.496C11.6192 17.7243 11.9186 17.8384 12.2183 17.8384Z" />
              </g>
              <defs>
                <clipPath id="clip0">
                  <rect width="40" height="40" fill="white"/>
                </clipPath>
              </defs>
            </svg>

            <p class="girl-profile-menu__item--text">未来广播</p>
          </div>
          <div class="girl-profile-menu__item ">
            <svg class="girl-profile-menu__item--img" width="38" height="40" viewBox="0 0 38 40" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M24.0197 12.3922L31.706 7.52943L24.1766 0L19.3139 10.8235L16.4903 2.35293L8.96094 7.37253L15.2354 12.3921H0.960938V22.4314H3.47074V40H34.5295V22.4314H37.0393V12.3922H24.0197ZM24.8116 3.29703L28.7514 7.23687L20.7148 12.3332L24.8116 3.29703ZM15.4839 5.2862L17.7085 11.9601L12.1469 7.51083L15.4839 5.2862ZM16.4903 37.4902H5.98054V21.6452H16.4903V37.4902ZM16.4903 19.9215H3.47074V14.902H16.4903V19.9215ZM32.0197 37.4902H21.5099V21.6452H32.0197V37.4902ZM34.5295 19.9215H21.5099V14.902H34.5295V19.9215Z" />
            </svg>

            <p class="girl-profile-menu__item--text">未来广播</p>
          </div>
        </div>

        <div v-show="activeTab==='userInfo'" class="girl-profile-wrapper">
          <div class="girl-profile-left">
            <div class="block-rounded border-orange">
              <div class="block-inner">
                <p class="section-subheader mb-30 text-orange">我的粉丝和赞助商</p>
                <img src="/testw.png" alt="">
              </div>
            </div>
            <div class="block-rounded p50">
              <p class="section-subheader mb-30 ">朋友们</p>
              <div class="girl-profile-friends">
                <img src="/testw.png" alt="">
                <img src="/testw.png" alt="">
                <img src="/testw.png" alt="">
                <img src="/testw.png" alt="">
                <img src="/testw.png" alt="">
                <img src="/testw.png" alt="">
                <img src="/testw.png" alt="">
                <div class="girl-profile-friends__more"><p>+ 999</p></div>
              </div>
            </div>
            <div class="block-rounded p50">
              <p class="section-subheader mb-30 ">我的团体</p>

              <div class="girl-profile-groups">
                <div class="girl-profile-group__item">
                  <div class="girl-profile-group__item--img">
                    <img src="/testw.png" alt="">
                  </div>
                  <div class="girl-profile-group__item--name">
                    <p>Best!Cute!Girls!<3</p>
                    <p>24 385 members</p>
                  </div>
                  <div class="girl-profile-group__item--btn">
                    <p>+</p>
                  </div>
                </div>
              </div>

            </div>
          </div>
          <div class="girl-profile-right">
            <div class="block-rounded p50">
              <p class="section-subheader mb-30">简要信息</p>
              <p class="mb-20">嗨！ 我的名字叫，但有些人可能将我称为GameHuntress！ 我有一个Twitch频道，可以在其中播放，播放和查看所有最新游戏。</p>
              <p class="mb-20">嗨！ 我的名字叫，但有些人可能将我称为GameHuntress！ 我有一个Twitch频道，可以在其中播放，播放和查看所有最新游戏。</p>
              <p >嗨！ 我的名字叫，但有些人可能将我称为GameHuntress！ 我有一个Twitch频道，可以在其中播放，播放和查看所有最新游戏。</p>

            </div>
            <div class="block-rounded p50">
              <p class="section-subheader mb-30">简要信息</p>
              <p class="mb-60">嗨！ 我的名字叫，但有些人可能将我称为GameHuntress！ 我有一个Twitch频道，可以在其中播放，播放和查看所有最新游戏。</p>
              <div class="profile-user-info">
                <p>已加入</p>
                <p>2020年3月26日</p>
              </div>
              <div class="profile-user-info">
                <p>市</p>
                <p>莫斯科</p>
              </div>
              <div class="profile-user-info">
                <p>国家</p>
                <p>俄罗斯联邦</p>
              </div>
              <div class="profile-user-info">
                <p>年龄</p>
                <p>24</p>
              </div>
            </div>
          </div>
        </div><!--        userInfoTab-->
        <div v-show="activeTab==='userFriends'" class="">
          <div class="models-wrapper">

                <div class="model-item">
                  <div class="model-item__bg" style="background: url(/test_bg.png)"></div>
                  <div class="model-item__img">
                    <img src="/test_w.png" alt="">
                  </div>
                  <p class="model-item__name">Alice Krystal</p>
                  <p class="model-item__login">@kistochka</p>

                  <div class="model-item__info">
                    <div class="model-item__info-left">
                      <p class="model-item__info-title">年龄</p>
                      <p class="model-item__info-text">24岁</p>
                    </div>
                    <div class="model-item__info-right">
                      <p class="model-item__info-title">兴趣爱好</p>
                      <p class="model-item__info-text">滑雪，乐透...</p>
                    </div>
                  </div>
                  <div class="model-item__buttons">
                    <div class="btn btn-blue btn-round"><p> 写短信</p></div>
                    <div class="btn btn-outline btn-outline-gold ">
                      <div class="btn-outline-inner">
                        <p>添加</p>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="model-item">
                  <div class="model-item__bg" style="background: url(/test_bg.png)"></div>
                  <div class="model-item__img">
                    <img src="/test_w.png" alt="">
                  </div>
                  <p class="model-item__name">Alice Krystal</p>
                  <p class="model-item__login">@kistochka</p>

                  <div class="model-item__info">
                    <div class="model-item__info-left">
                      <p class="model-item__info-title">年龄</p>
                      <p class="model-item__info-text">24岁</p>
                    </div>
                    <div class="model-item__info-right">
                      <p class="model-item__info-title">兴趣爱好</p>
                      <p class="model-item__info-text">滑雪，乐透...</p>
                    </div>
                  </div>
                  <div class="model-item__buttons">
                    <div class="btn btn-blue btn-round"><p> 写短信</p></div>
                    <div class="btn btn-outline btn-outline-gold ">
                      <div class="btn-outline-inner">
                        <p>添加</p>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="model-item">
                  <div class="model-item__bg" style="background: url(/test_bg.png)"></div>
                  <div class="model-item__img">
                    <img src="/test_w.png" alt="">
                  </div>
                  <p class="model-item__name">Alice Krystal</p>
                  <p class="model-item__login">@kistochka</p>

                  <div class="model-item__info">
                    <div class="model-item__info-left">
                      <p class="model-item__info-title">年龄</p>
                      <p class="model-item__info-text">24岁</p>
                    </div>
                    <div class="model-item__info-right">
                      <p class="model-item__info-title">兴趣爱好</p>
                      <p class="model-item__info-text">滑雪，乐透...</p>
                    </div>
                  </div>
                  <div class="model-item__buttons">
                    <div class="btn btn-blue btn-round"><p> 写短信</p></div>
                    <div class="btn btn-outline btn-outline-gold ">
                      <div class="btn-outline-inner">
                        <p>添加</p>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="model-item">
                  <div class="model-item__bg" style="background: url(/test_bg.png)"></div>
                  <div class="model-item__img">
                    <img src="/test_w.png" alt="">
                  </div>
                  <p class="model-item__name">Alice Krystal</p>
                  <p class="model-item__login">@kistochka</p>

                  <div class="model-item__info">
                    <div class="model-item__info-left">
                      <p class="model-item__info-title">年龄</p>
                      <p class="model-item__info-text">24岁</p>
                    </div>
                    <div class="model-item__info-right">
                      <p class="model-item__info-title">兴趣爱好</p>
                      <p class="model-item__info-text">滑雪，乐透...</p>
                    </div>
                  </div>
                  <div class="model-item__buttons">
                    <div class="btn btn-blue btn-round"><p> 写短信</p></div>
                    <div class="btn btn-outline btn-outline-gold ">
                      <div class="btn-outline-inner">
                        <p>添加</p>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="model-item">
                  <div class="model-item__bg" style="background: url(/test_bg.png)"></div>
                  <div class="model-item__img">
                    <img src="/test_w.png" alt="">
                  </div>
                  <p class="model-item__name">Alice Krystal</p>
                  <p class="model-item__login">@kistochka</p>

                  <div class="model-item__info">
                    <div class="model-item__info-left">
                      <p class="model-item__info-title">年龄</p>
                      <p class="model-item__info-text">24岁</p>
                    </div>
                    <div class="model-item__info-right">
                      <p class="model-item__info-title">兴趣爱好</p>
                      <p class="model-item__info-text">滑雪，乐透...</p>
                    </div>
                  </div>
                  <div class="model-item__buttons">
                    <div class="btn btn-blue btn-round"><p> 写短信</p></div>
                    <div class="btn btn-outline btn-outline-gold ">
                      <div class="btn-outline-inner">
                        <p>添加</p>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="model-item">
                  <div class="model-item__bg" style="background: url(/test_bg.png)"></div>
                  <div class="model-item__img">
                    <img src="/test_w.png" alt="">
                  </div>
                  <p class="model-item__name">Alice Krystal</p>
                  <p class="model-item__login">@kistochka</p>

                  <div class="model-item__info">
                    <div class="model-item__info-left">
                      <p class="model-item__info-title">年龄</p>
                      <p class="model-item__info-text">24岁</p>
                    </div>
                    <div class="model-item__info-right">
                      <p class="model-item__info-title">兴趣爱好</p>
                      <p class="model-item__info-text">滑雪，乐透...</p>
                    </div>
                  </div>
                  <div class="model-item__buttons">
                    <div class="btn btn-blue btn-round"><p> 写短信</p></div>
                    <div class="btn btn-outline btn-outline-gold ">
                      <div class="btn-outline-inner">
                        <p>添加</p>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
        </div><!--        userFriends-->
        <div v-show="activeTab==='userGallery'" class="girl-profile-gallery">
          <p class="section-subheader mb-50">专辑 3</p>
          <div class="girl-profile-albums">
            <div class="girl-profile-album" style="background:linear-gradient(black, black), url(/test.png) no-repeat center">
              <div class="girl-profile-album__counter">
                <p>47</p></div>
              <div class="girl-profile-album__title">个人资料照片</div>
              <div class="girl-profile-album__subtitle">1周前更新</div>
            </div>
            <div class="girl-profile-album  " style="background:linear-gradient(black, black), url(/test.png) no-repeat center">
              <div class="girl-profile-album__locked">
                <img src="/stream_for_vip_icon.png" alt="">
              </div>
              <div class="girl-profile-album__counter">
                <p>47</p></div>
              <div class="girl-profile-album__title">个人资料照片</div>
              <div class="girl-profile-album__subtitle">1周前更新</div>
            </div>
            <div class="girl-profile-album" style="background: url(http://placehold.it/310) no-repeat center">
              <div class="girl-profile-album__counter">
                <p>47</p></div>
              <div class="girl-profile-album__title">个人资料照片</div>
              <div class="girl-profile-album__subtitle">1周前更新</div>
            </div>
            <div class="girl-profile-album" style="background: url(http://placehold.it/310) no-repeat center">
              <div class="girl-profile-album__counter">
                <p>47</p></div>
              <div class="girl-profile-album__title">个人资料照片</div>
              <div class="girl-profile-album__subtitle">1周前更新</div>
            </div>
          </div>
          <p class="section-subheader mb-50">VIP专辑 1</p>
          <div class="girl-profile-albums">
            <div class="girl-profile-album vipAlbum " style="background:linear-gradient(black, black), url(/test.png) no-repeat center">
              <div class="girl-profile-album__locked">
                <img src="/stream_for_vip_icon.png" alt="">
              </div>
              <div class="girl-profile-album__counter">
                <p>47</p></div>
              <div class="girl-profile-album__title">个人资料照片</div>
              <div class="girl-profile-album__subtitle">1周前更新</div>
            </div>

          </div>

          <p class="section-subheader mb-50">最后一张照片 34</p>
          <div class="girl-profile-album-content">
            <div @click="currentImage='http://placehold.it/1000x1000',imageModal=true" class="girl-profile-album-content__item">
              <img src="/test.png" alt="">
            </div>
            <div class="girl-profile-album-content__item">
              <img src="https://picsum.photos/400/400?image=255" alt="">
            </div>
            <div class="girl-profile-album-content__item">
              <img src="https://picsum.photos/400/400?image=255" alt="">
            </div>
            <div class="girl-profile-album-content__item">
              <img src="https://picsum.photos/400/400?image=255" alt="">
            </div>
            <div class="girl-profile-album-content__item">
              <img src="https://picsum.photos/400/400?image=255" alt="">
            </div>
            <div class="girl-profile-album-content__item">
              <img src="https://picsum.photos/400/400?image=255" alt="">
            </div>
          </div>

          <vs-popup class="holamundo"   :active.sync="imageModal">
            <img :src="currentImage" alt="">
          </vs-popup>
        </div><!--        userGalleryTab-->
        <div v-show="activeTab==='userStreamTab'" class="">
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
        </div><!--        userStreamTab-->
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
        activeTab:'userInfo',//'userInfo'
        imageModal:false,
        currentImage:null,
      }
    },

    methods:{
      showImage(image){
        console.log(image)
      },

    }
  }
</script>


<style >
  .my-player-dimensions{
    width: 100%;
  }
  .vs-popup--header{
    display: none !important
  }
  .con-vs-popup .vs-popup{
    /*width: 320px !important;*/
  }
  .fade-enter {
    transition: all .5s ease-in-out;
    opacity: 0;
    transform :  translateX(100px);


  }
  .fade-enter-to {
    transition: all .5s ease-in-out;
    opacity: 1;
    transform :  translateX(0px);

  }

  .fade-leave {
    transition: all .5s ease-in-out;
    opacity: 0;
    transform :  translateX(0px);

  }
  .fade-leave-to {
    transition: all .5s ease-in-out;
    opacity: 1;
    transform :  translateX(0px);

  }
  /*.fade-leave-active{*/
  /*  transition: all .5s ease-in-out;*/
  /*  opacity: 0;*/
  /*}*/
  /*.fade-enter, .fade-leave-to  {*/
  /*  opacity: 0;*/
  /*  transform :  translateX(100px);*/
  /*}*/
</style>
