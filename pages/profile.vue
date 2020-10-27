<template>
  <div>
    <section class="profile">
      <div class="container">
        <div class="profile-user-area">
          <div class="profile-user-area__img" style="background: url(/test_profile_m_bg.png) no-repeat center"></div>
          <div class="profile-user-area__avatar">
            <img src="https://picsum.photos/400/400?image=27" alt="">
          </div>
          <div class="profile-user-area__info">
            <div class="profile-user-area__info--name">
              <p>li pin hin</p>
              <p><a href="#">@promoman</a></p>
            </div>
            <div class="profile-user-area__info--buttons">
              <div class="btn btn-blue btn-round"><p>text</p></div>
              <div class="btn btn-blue btn-round"><p>text</p></div>
            </div>
          </div>
        </div>
        <div class="profile-wrapper">
          <div class="profile-left">
            <div class="profile-menu">
              <ul>
                <!--                itemActive-->
                <li class="profile-menu__item " @click="activeTab='userInfo'" :class="{'itemActive':activeTab==='userInfo'}">
                  <svg class="profile-menu__item--img" width="26" height="26" viewBox="0 0 28 28" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M26.1817 22.8453C25.5185 21.2744 24.5561 19.8475 23.3481 18.6441C22.1438 17.4373 20.7171 16.475 19.147 15.8105C19.1329 15.8035 19.1188 15.8 19.1048 15.793C21.295 14.2109 22.7188 11.634 22.7188 8.72656C22.7188 3.91016 18.8165 0.0078125 14.0001 0.0078125C9.18368 0.0078125 5.28134 3.91016 5.28134 8.72656C5.28134 11.634 6.70517 14.2109 8.8954 15.7965C8.88134 15.8035 8.86728 15.807 8.85321 15.8141C7.27821 16.4785 5.86493 17.4312 4.65204 18.6477C3.44516 19.852 2.48292 21.2786 1.81845 22.8488C1.16567 24.386 0.813618 26.0341 0.781338 27.7039C0.7804 27.7414 0.786981 27.7788 0.800694 27.8137C0.814408 27.8486 0.834976 27.8805 0.861186 27.9073C0.887397 27.9342 0.918719 27.9556 0.953309 27.9701C0.987898 27.9847 1.02505 27.9922 1.06259 27.9922H3.17196C3.32665 27.9922 3.4497 27.8691 3.45321 27.718C3.52353 25.0039 4.61337 22.4621 6.53993 20.5355C8.53329 18.5422 11.1806 17.4453 14.0001 17.4453C16.8196 17.4453 19.4669 18.5422 21.4602 20.5355C23.3868 22.4621 24.4767 25.0039 24.547 27.718C24.5505 27.8727 24.6735 27.9922 24.8282 27.9922H26.9376C26.9751 27.9922 27.0123 27.9847 27.0469 27.9701C27.0815 27.9556 27.1128 27.9342 27.139 27.9073C27.1652 27.8805 27.1858 27.8486 27.1995 27.8137C27.2132 27.7788 27.2198 27.7414 27.2188 27.7039C27.1837 26.0234 26.8356 24.3887 26.1817 22.8453ZM14.0001 14.7734C12.3864 14.7734 10.8677 14.1441 9.72509 13.0016C8.58251 11.859 7.95321 10.3402 7.95321 8.72656C7.95321 7.11289 8.58251 5.59414 9.72509 4.45156C10.8677 3.30898 12.3864 2.67969 14.0001 2.67969C15.6138 2.67969 17.1325 3.30898 18.2751 4.45156C19.4177 5.59414 20.047 7.11289 20.047 8.72656C20.047 10.3402 19.4177 11.859 18.2751 13.0016C17.1325 14.1441 15.6138 14.7734 14.0001 14.7734Z" />
                  </svg>
                  <p class="profile-menu__item--text">我的简历</p>
                </li>
                <li class="profile-menu__item" @click="activeTab='userFriends'" :class="{'itemActive':activeTab==='userFriends'}">
                  <svg class="profile-menu__item--img" width="26" height="26" viewBox="0 0 34 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M9.125 0.875C5.4125 0.875 2.375 3.9125 2.375 7.625C2.375 9.857 3.47412 11.8438 5.15263 13.0745C2.186 14.546 0.125 17.597 0.125 21.125H2.375C2.375 17.3855 5.3855 14.375 9.125 14.375C12.8645 14.375 15.875 17.3855 15.875 21.125H18.125C18.125 17.3855 21.1355 14.375 24.875 14.375C28.6145 14.375 31.625 17.3855 31.625 21.125H33.875C33.875 17.5959 31.814 14.546 28.8474 13.0745C29.7063 12.4486 30.4055 11.6289 30.8881 10.682C31.3708 9.73517 31.6232 8.68779 31.625 7.625C31.625 3.9125 28.5875 0.875 24.875 0.875C21.1625 0.875 18.125 3.9125 18.125 7.625C18.125 9.857 19.2241 11.8438 20.9026 13.0745C19.2589 13.8826 17.8984 15.1695 17 16.7656C16.1016 15.1695 14.7411 13.8826 13.0974 13.0745C13.9563 12.4486 14.6555 11.6289 15.1381 10.682C15.6208 9.73517 15.8732 8.68779 15.875 7.625C15.875 3.9125 12.8375 0.875 9.125 0.875ZM9.125 3.125C11.6259 3.125 13.625 5.12413 13.625 7.625C13.625 10.1259 11.6259 12.125 9.125 12.125C6.62413 12.125 4.625 10.1259 4.625 7.625C4.625 5.12413 6.62413 3.125 9.125 3.125ZM24.875 3.125C27.3759 3.125 29.375 5.12413 29.375 7.625C29.375 10.1259 27.3759 12.125 24.875 12.125C22.3741 12.125 20.375 10.1259 20.375 7.625C20.375 5.12413 22.3741 3.125 24.875 3.125Z" />
                  </svg>

                  <p class="profile-menu__item--text">我的朋友名单</p>
                </li>
                <li class="profile-menu__item " @click="activeTab='userSettings'" :class="{'itemActive':activeTab==='userSettings'}">
                  <svg class="profile-menu__item--img" width="26" height="26" viewBox="0 0 36 36" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M30.3754 18.8553V18.0003V17.1341L32.5354 15.2441C32.9336 14.8931 33.1949 14.4127 33.2731 13.8878C33.3513 13.3628 33.2414 12.8271 32.9629 12.3753L30.3079 7.87534C30.1106 7.53363 29.827 7.24981 29.4853 7.05235C29.1437 6.8549 28.7562 6.75074 28.3617 6.75034C28.1171 6.74846 27.8739 6.78646 27.6417 6.86284L24.9079 7.78534C24.4359 7.47169 23.9436 7.18982 23.4342 6.94159L22.8604 4.10659C22.7575 3.58864 22.4758 3.12338 22.0644 2.79225C21.6531 2.46112 21.1384 2.28522 20.6104 2.29534H15.3454C14.8174 2.28522 14.3027 2.46112 13.8914 2.79225C13.4801 3.12338 13.1983 3.58864 13.0954 4.10659L12.5217 6.94159C12.0086 7.18976 11.5125 7.47163 11.0367 7.78534L8.35916 6.81784C8.12437 6.75666 7.88123 6.73387 7.63916 6.75034C7.24459 6.75074 6.85707 6.8549 6.51546 7.05235C6.17386 7.24981 5.89019 7.53363 5.69291 7.87534L3.03791 12.3753C2.77532 12.8264 2.67774 13.3548 2.76189 13.87C2.84603 14.3851 3.10667 14.855 3.49916 15.1991L5.62541 17.1453V18.8666L3.49916 20.7566C3.09558 21.1031 2.82782 21.5814 2.74338 22.1065C2.65894 22.6317 2.76329 23.1698 3.03791 23.6253L5.69291 28.1253C5.89019 28.467 6.17386 28.7509 6.51546 28.9483C6.85707 29.1458 7.24459 29.2499 7.63916 29.2503C7.88368 29.2522 8.12686 29.2142 8.35916 29.1378L11.0929 28.2153C11.5649 28.529 12.0572 28.8109 12.5667 29.0591L13.1404 31.8941C13.2433 32.412 13.5251 32.8773 13.9364 33.2084C14.3477 33.5395 14.8624 33.7155 15.3904 33.7053H20.7004C21.2284 33.7155 21.7431 33.5395 22.1544 33.2084C22.5658 32.8773 22.8475 32.412 22.9504 31.8941L23.5242 29.0591C24.0372 28.8109 24.5333 28.529 25.0092 28.2153L27.7317 29.1378C27.9639 29.2142 28.2071 29.2522 28.4517 29.2503C28.8462 29.2499 29.2337 29.1458 29.5753 28.9483C29.917 28.7509 30.2006 28.467 30.3979 28.1253L32.9629 23.6253C33.2255 23.1742 33.3231 22.6458 33.2389 22.1307C33.1548 21.6156 32.8941 21.1457 32.5017 20.8016L30.3754 18.8553ZM28.3617 27.0003L24.5029 25.6953C23.5996 26.4605 22.5672 27.0585 21.4542 27.4616L20.6554 31.5003H15.3454L14.5467 27.5066C13.4424 27.0921 12.4156 26.495 11.5092 25.7403L7.63916 27.0003L4.98416 22.5003L8.04416 19.8003C7.83614 18.6358 7.83614 17.4436 8.04416 16.2791L4.98416 13.5003L7.63916 9.00034L11.4979 10.3053C12.4012 9.54021 13.4336 8.94212 14.5467 8.53909L15.3454 4.50034H20.6554L21.4542 8.49409C22.5584 8.90856 23.5852 9.50562 24.4917 10.2603L28.3617 9.00034L31.0167 13.5003L27.9567 16.2003C28.1647 17.3649 28.1647 18.5571 27.9567 19.7216L31.0167 22.5003L28.3617 27.0003Z" />
                    <path d="M18 24.75C16.665 24.75 15.3599 24.3541 14.2499 23.6124C13.1399 22.8707 12.2747 21.8165 11.7638 20.5831C11.2529 19.3497 11.1193 17.9925 11.3797 16.6831C11.6402 15.3738 12.283 14.171 13.227 13.227C14.171 12.283 15.3738 11.6402 16.6831 11.3797C17.9925 11.1193 19.3497 11.2529 20.5831 11.7638C21.8165 12.2747 22.8707 13.1399 23.6124 14.2499C24.3541 15.3599 24.75 16.665 24.75 18C24.759 18.8889 24.5906 19.7707 24.2546 20.5938C23.9185 21.4168 23.4217 22.1645 22.7931 22.7931C22.1645 23.4217 21.4168 23.9185 20.5938 24.2546C19.7707 24.5906 18.8889 24.759 18 24.75ZM18 13.5C17.4053 13.4861 16.8139 13.5931 16.2617 13.8143C15.7094 14.0356 15.2078 14.3665 14.7872 14.7872C14.3665 15.2078 14.0356 15.7094 13.8143 16.2617C13.5931 16.8139 13.4861 17.4053 13.5 18C13.4861 18.5947 13.5931 19.1861 13.8143 19.7383C14.0356 20.2906 14.3665 20.7922 14.7872 21.2128C15.2078 21.6335 15.7094 21.9644 16.2617 22.1857C16.8139 22.4069 17.4053 22.5139 18 22.5C18.5947 22.5139 19.1861 22.4069 19.7383 22.1857C20.2906 21.9644 20.7922 21.6335 21.2128 21.2128C21.6335 20.7922 21.9644 20.2906 22.1857 19.7383C22.4069 19.1861 22.5139 18.5947 22.5 18C22.5139 17.4053 22.4069 16.8139 22.1857 16.2617C21.9644 15.7094 21.6335 15.2078 21.2128 14.7872C20.7922 14.3665 20.2906 14.0356 19.7383 13.8143C19.1861 13.5931 18.5947 13.4861 18 13.5Z" />
                  </svg>


                  <p class="profile-menu__item--text">我的设置和费率</p>
                </li>
                <li class="profile-menu__item" @click="activeTab='userFavorites'" :class="{'itemActive':activeTab==='userFavorites'}">
                  <svg class="profile-menu__item--img" width="26" height="26" viewBox="0 0 30 29" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M21.75 0.5C19.14 0.5 16.635 1.715 15 3.635C13.365 1.715 10.86 0.5 8.25 0.5C3.63 0.5 0 4.13 0 8.75C0 14.42 5.1 19.04 12.825 26.06L15 28.025L17.175 26.045C24.9 19.04 30 14.42 30 8.75C30 4.13 26.37 0.5 21.75 0.5ZM15.15 23.825L15 23.975L14.85 23.825C7.71 17.36 3 13.085 3 8.75C3 5.75 5.25 3.5 8.25 3.5C10.56 3.5 12.81 4.985 13.605 7.04H16.41C17.19 4.985 19.44 3.5 21.75 3.5C24.75 3.5 27 5.75 27 8.75C27 13.085 22.29 17.36 15.15 23.825Z" />
                  </svg>

                  <p class="profile-menu__item--text">广播评级</p>
                </li>
                <li class="profile-menu__item " @click="activeTab='userChat'" :class="{'itemActive':activeTab==='userChat'}">
                  <svg class="profile-menu__item--img" width="26" height="26" viewBox="0 0 34 34" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M30.3894 26.4731C32.5353 24.5606 33.7504 22.0115 33.7504 19.3661C33.7504 16.5547 32.4342 13.9255 30.0444 11.9622C27.7185 10.0521 24.6398 9 21.375 9C18.1103 9 15.0315 10.0521 12.706 11.9623C10.3161 13.9255 9 16.5547 9 19.3661C9 22.1775 10.3161 24.8067 12.706 26.77C15.0315 28.6803 18.1103 29.7323 21.375 29.7323C21.81 29.7323 22.2477 29.7131 22.6818 29.6749L23.4233 30.3176C25.9778 32.5313 29.2448 33.7499 32.625 33.75H33.75V31.3554L33.4205 31.026C32.1207 29.7223 31.0907 28.1752 30.3894 26.4731ZM24.8969 28.6172L23.409 27.3276L22.9129 27.3884C22.4026 27.4508 21.8891 27.4821 21.375 27.4821C15.7922 27.4821 11.25 23.8413 11.25 19.3661C11.25 14.8909 15.7922 11.25 21.375 11.25C26.9578 11.25 31.5 14.8909 31.5 19.3661C31.5 21.5957 30.3877 23.6772 28.3679 25.2272L27.7199 25.7244L28.0189 26.5706C28.6316 28.2989 29.5321 29.9111 30.6825 31.339C28.5402 30.9814 26.5382 30.0396 24.8969 28.6172Z" />
                    <path d="M3.10676 21.1975C4.15985 19.8645 4.98668 18.3674 5.55419 16.7662L5.85091 15.9242L5.20355 15.4274C3.29892 13.9659 2.25 12.0043 2.25 9.90401C2.25 5.68357 6.5397 2.25 11.8125 2.25C15.6915 2.25 19.0383 4.10836 20.5367 6.77109C20.8149 6.75759 21.0943 6.75 21.375 6.75C21.9388 6.75 22.4974 6.77735 23.0508 6.83205C22.4718 5.33194 21.4662 3.96253 20.0836 2.82698C17.8644 1.00399 14.9273 0 11.8125 0C8.69766 0 5.76056 1.00399 3.54122 2.82698C1.25761 4.70285 0 7.21617 0 9.90401C0 12.4212 1.14975 14.8466 3.18164 16.6711C2.51855 18.2668 1.54966 19.7174 0.329555 20.9411L0 21.2706V23.625H1.125C3.20534 23.6247 5.25707 23.1403 7.11781 22.21C6.91377 21.4366 6.79422 20.6434 6.76125 19.8443C5.63187 20.5062 4.39486 20.9643 3.10676 21.1975Z" />
                  </svg>

                  <p class="profile-menu__item--text">聊天室</p>
                </li>
              </ul>
            </div>
            <div class="btn btn-orange btn-w-img">
              <svg width="26" height="26" viewBox="0 0 32 28" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M3.34138 9.21389L5.25474 25.0953H26.7451L28.6584 9.21389L22.6922 13.096L15.9999 3.95058L9.30761 13.096L3.34138 9.21389ZM2.31328 5.05291L8.56071 9.11948L14.7888 0.60873C14.9264 0.420461 15.1081 0.267 15.3188 0.16112C15.5294 0.0552389 15.763 0 15.9999 0C16.2368 0 16.4704 0.0552389 16.681 0.16112C16.8917 0.267 17.0734 0.420461 17.211 0.60873L23.4391 9.11948L29.688 5.05291C29.9245 4.89932 30.2011 4.81503 30.4851 4.80999C30.7691 4.80495 31.0487 4.87938 31.2907 5.02448C31.5328 5.16958 31.7273 5.37929 31.8511 5.62882C31.975 5.87835 32.0231 6.15728 31.9897 6.43264L29.5452 26.7176C29.5026 27.0709 29.3286 27.3966 29.0562 27.633C28.7839 27.8694 28.4322 28 28.0678 28H3.93205C3.56763 28 3.2159 27.8694 2.94357 27.633C2.67124 27.3966 2.49726 27.0709 2.45462 26.7176L0.0101049 6.43119C-0.0229251 6.15595 0.0254075 5.87722 0.149397 5.62792C0.273387 5.37862 0.467857 5.16915 0.709852 5.02424C0.951846 4.87933 1.23126 4.80503 1.51511 4.81011C1.79896 4.81519 2.0754 4.89944 2.31179 5.05291H2.31328ZM15.9999 19.2859C15.2107 19.2859 14.4538 18.9799 13.8958 18.4352C13.3377 17.8904 13.0242 17.1516 13.0242 16.3812C13.0242 15.6108 13.3377 14.872 13.8958 14.3273C14.4538 13.7826 15.2107 13.4765 15.9999 13.4765C16.7891 13.4765 17.546 13.7826 18.104 14.3273C18.6621 14.872 18.9756 15.6108 18.9756 16.3812C18.9756 17.1516 18.6621 17.8904 18.104 18.4352C17.546 18.9799 16.7891 19.2859 15.9999 19.2859Z" fill="white"/>
              </svg>
              <p>
                VIP 我的简历
              </p>
            </div>
          </div>
          <transition name = "fade">
            <div v-show="activeTab==='userInfo'" class="profile-right">
              <div @click="activeTab='userVip'" class="block-rounded p20 profile-balance">
                <img src="/profile-balance-icon.png" alt="">
                <p class="profile-balance__amount text-blue">2350</p>
                <p class="profile-balance__text">我的余额</p>
                <div class="btn btn-outline btn-outline-blue">
                  <div class="btn-outline-inner">
                    <p>
                      申请申请
                    </p>
                  </div>
                </div>
                <div class="btn btn-blue btn-round">
                  <p>申请</p>
                </div>
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
              <div class="block-rounded p50">
                <p class="section-subheader mb-30">简要信息</p>
                <div class="profile-user-info__form">
                  <div class="">
                    <vs-input style="width: 100%" size="default" label-placeholder="简要信息简要信息" v-model="value1"/>
                    <vs-input style="width: 100%" label-placeholder="简要信息简要信息" v-model="value2"/>
                  </div>
                  <div class="">
                    <vs-input style="width: 100%" size="default" label-placeholder="简要信息简要信息" v-model="value1"/>
                    <vs-input style="width: 100%" label-placeholder="简要信息简要信息" v-model="value2"/>
                  </div>
                </div>
                <div class="btn btn-outline btn-outline-blue">
                  <div class="btn-outline-inner">
                    <p>申请</p>
                  </div>
                </div>

              </div>
            </div>
          </transition>
          <transition name = "fade">
            <div v-show="activeTab==='userFriends'" class="profile-right">
              <div class="block-rounded p20 profile-balance">
                <img src="/profile-balance-icon.png" alt="">
                <p class="profile-balance__amount text-blue">2350</p>
                <p class="profile-balance__text">我的余额</p>

                <div class="btn btn-outline btn-outline-blue">
                  <div class="btn-outline-inner">
                    <p>
                      申请申请
                    </p>
                  </div>
                </div>
                <div class="btn btn-blue btn-round">
                  <p>申请</p>
                </div>


              </div>
              <div class="models-wrapper">

                 <div class="model-item">
            <nuxt-link to="/girl-profile">
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
            </nuxt-link>
          </div>
                  <div class="model-item">
            <nuxt-link to="/girl-profile">
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
            </nuxt-link>
          </div>
                  <div class="model-item">
            <nuxt-link to="/girl-profile">
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
            </nuxt-link>
          </div>
              </div>
            </div>
          </transition>
          <transition name = "fade">
            <div v-show="activeTab==='userFavorites'" class="profile-right">
              <div class="block-rounded p20 profile-balance">
                <img src="/profile-balance-icon.png" alt="">
                <p class="profile-balance__amount text-blue">2350</p>
                <p class="profile-balance__text">我的余额</p>

                <div class="btn btn-outline btn-outline-blue">
                  <div class="btn-outline-inner">
                    <p>
                      申请申请
                    </p>
                  </div>
                </div>
                <div class="btn btn-blue btn-round">
                  <p>申请</p>
                </div>


              </div>
              <div class="groups-wrapper">

                  <div class="group-item">
            <nuxt-link to="/group-profile">
              <div class="group-item__top" style="background: url(/test_g_bg.png)"></div>
              <div class="group-item__button">
                <img draggable="false" src="/group_icon.png" alt="">
              </div>
              <div class="group-item__img">
                <img draggable="false" src="https://www.wotcheatmods.com/wp-content/uploads/2020/04/440_wot_premium.png" alt="">
              </div>
              <div class="group-item__title">我们爱坦克世界</div>
              <div class="group-item__subtitle">广播评级广播评级</div>
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
            </nuxt-link>
          </div>
                  <div class="group-item">
            <nuxt-link to="/group-profile">
              <div class="group-item__top" style="background: url(/test_g_bg.png)"></div>
              <div class="group-item__button">
                <img draggable="false" src="/group_icon.png" alt="">
              </div>
              <div class="group-item__img">
                <img draggable="false" src="https://www.wotcheatmods.com/wp-content/uploads/2020/04/440_wot_premium.png" alt="">
              </div>
              <div class="group-item__title">我们爱坦克世界</div>
              <div class="group-item__subtitle">广播评级广播评级</div>
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
            </nuxt-link>
          </div>
                  <div class="group-item">
            <nuxt-link to="/group-profile">
              <div class="group-item__top" style="background: url(/test_g_bg.png)"></div>
              <div class="group-item__button">
                <img draggable="false" src="/group_icon.png" alt="">
              </div>
              <div class="group-item__img">
                <img draggable="false" src="https://www.wotcheatmods.com/wp-content/uploads/2020/04/440_wot_premium.png" alt="">
              </div>
              <div class="group-item__title">我们爱坦克世界</div>
              <div class="group-item__subtitle">广播评级广播评级</div>
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
            </nuxt-link>
          </div>
                  <div class="group-item">
            <nuxt-link to="/group-profile">
              <div class="group-item__top" style="background: url(/test_g_bg.png)"></div>
              <div class="group-item__button">
                <img draggable="false" src="/group_icon.png" alt="">
              </div>
              <div class="group-item__img">
                <img draggable="false" src="https://www.wotcheatmods.com/wp-content/uploads/2020/04/440_wot_premium.png" alt="">
              </div>
              <div class="group-item__title">我们爱坦克世界</div>
              <div class="group-item__subtitle">广播评级广播评级</div>
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
            </nuxt-link>
          </div>
                  <div class="group-item">
            <nuxt-link to="/group-profile">
              <div class="group-item__top" style="background: url(/test_g_bg.png)"></div>
              <div class="group-item__button">
                <img draggable="false" src="/group_icon.png" alt="">
              </div>
              <div class="group-item__img">
                <img draggable="false" src="https://www.wotcheatmods.com/wp-content/uploads/2020/04/440_wot_premium.png" alt="">
              </div>
              <div class="group-item__title">我们爱坦克世界</div>
              <div class="group-item__subtitle">广播评级广播评级</div>
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
            </nuxt-link>
          </div>
                  <div class="group-item">
            <nuxt-link to="/group-profile">
              <div class="group-item__top" style="background: url(/test_g_bg.png)"></div>
              <div class="group-item__button">
                <img draggable="false" src="/group_icon.png" alt="">
              </div>
              <div class="group-item__img">
                <img draggable="false" src="https://www.wotcheatmods.com/wp-content/uploads/2020/04/440_wot_premium.png" alt="">
              </div>
              <div class="group-item__title">我们爱坦克世界</div>
              <div class="group-item__subtitle">广播评级广播评级</div>
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
            </nuxt-link>
          </div>
              </div>
            </div>
          </transition>
          <transition name = "fade">
            <div v-show="activeTab==='userSettings'" class="profile-right">
              <div class="block-rounded p20 profile-balance">
                <img src="/profile-balance-icon.png" alt="">
                <p class="profile-balance__amount text-blue">2350</p>
                <p class="profile-balance__text">我的余额</p>

                <div class="btn btn-outline btn-outline-blue">
                  <div class="btn-outline-inner">
                    <p>
                      申请申请
                    </p>
                  </div>
                </div>
                <div class="btn btn-blue btn-round">
                  <p>申请</p>
                </div>


              </div>
                <div class="block-rounded p50">
                <p class="section-subheader mb-30">简要信息</p>
                  <div style="display: flex;align-items: center;justify-content: flex-start">
                     <vs-upload style="margin-right: 20px" action="https://jsonplaceholder.typicode.com/posts/" text="Change avatar" :show-upload-button="false" @on-success="successUpload" />
                   <vs-upload action="https://jsonplaceholder.typicode.com/posts/" text="Change BG" :show-upload-button="false" @on-success="successUpload" />
                  </div>
                  <div class="profile-user-info__form">
                  <div class="">
                    <vs-input style="width: 100%" size="default" label-placeholder="简要信息简要信息" v-model="value1"/>
                    <vs-input style="width: 100%" label-placeholder="简要信息简要信息" v-model="value2"/>
                    <vs-input style="width: 100%" size="default" label-placeholder="简要信息简要信息" v-model="value1"/>
                    <vs-input style="width: 100%" label-placeholder="简要信息简要信息" v-model="value2"/>
                  </div>
                  <div class="">
                    <vs-input style="width: 100%" size="default" label-placeholder="简要信息简要信息" v-model="value1"/>
                    <vs-input style="width: 100%" label-placeholder="简要信息简要信息" v-model="value2"/>
                    <vs-input style="width: 100%" size="default" label-placeholder="简要信息简要信息" v-model="value1"/>
                    <vs-input style="width: 100%" label-placeholder="简要信息简要信息" v-model="value2"/>
                  </div>
                </div>
                <div class="btn btn-outline btn-outline-blue">
                  <div class="btn-outline-inner">
                    <p>申请</p>
                  </div>
                </div>
              </div>
            </div>
          </transition>
          <transition name = "fade">
            <div v-show="activeTab==='userChat'" class="profile-right">
              <div class="block-rounded p20 profile-balance">
                <img src="/profile-balance-icon.png" alt="">
                <p class="profile-balance__amount text-blue">2350</p>
                <p class="profile-balance__text">我的余额</p>

                <div class="btn btn-outline btn-outline-blue">
                  <div class="btn-outline-inner">
                    <p>
                      申请申请
                    </p>
                  </div>
                </div>
                <div class="btn btn-blue btn-round">
                  <p>申请</p>
                </div>


              </div>
              <div class="chat-wrapper">
                <div class="chat-left">
                  <div class="chat-users">
                    <ul>
                      <!--                chatItemActive-->
                      <li class="chat-users__item chatItemActive">
                        <img class="chat-users__item--img" src="https://picsum.photos/400/400?image=24" alt="">
                        <div class="chat-users__item--lastMsg">
                          <p class="chat-users__item--text">我的简历</p>
                          <p class="chat-users__item--msg">fdgdvbcvbcvb  </p>
                        </div>
                        <p class="chat-users__item--time">10:30 10.09</p>
                      </li>
                      <li class="chat-users__item ">
                        <img class="chat-users__item--img" src="https://picsum.photos/400/400?image=56" alt="">
                        <div class="chat-users__item--lastMsg">
                          <p class="chat-users__item--text">我的简历</p>
                          <p class="chat-users__item--msg">fdgdfgfdg </p>
                        </div>
                        <p class="chat-users__item--time">10:30 10.09</p>
                      </li>
                      <li class="chat-users__item ">
                        <img class="chat-users__item--img" src="https://picsum.photos/400/400?image=53" alt="">
                        <div class="chat-users__item--lastMsg">
                          <p class="chat-users__item--text">我的简历</p>
                          <p class="chat-users__item--msg">fdgdfgfdg </p>
                        </div>
                        <p class="chat-users__item--time">10:30 10.09</p>
                      </li>
                      <li class="chat-users__item ">
                        <img class="chat-users__item--img" src="https://picsum.photos/400/400?image=50" alt="">
                        <div class="chat-users__item--lastMsg">
                          <p class="chat-users__item--text">我的简历</p>
                          <p class="chat-users__item--msg">fdgdfgfdg </p>
                        </div>
                        <p class="chat-users__item--time">10:30 10.09</p>
                      </li>
                      <li class="chat-users__item ">
                        <img class="chat-users__item--img" src="https://picsum.photos/400/400?image=76" alt="">
                        <div class="chat-users__item--lastMsg">
                          <p class="chat-users__item--text">我的简历</p>
                          <p class="chat-users__item--msg">fdgdfgfdg </p>
                        </div>
                        <p class="chat-users__item--time">10:30 10.09</p>
                      </li>

                    </ul>
                  </div>
                </div>
                <div class="chat-right ">
                  <div class="chat-content">
                    <div class="chat-content-msg">
                      <div class="chat-content-msg__item">
                        <img class="chat-content-msg__item--img" src="https://picsum.photos/400/400?image=73" alt="">
                        <p class="chat-content-msg__item--text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium alias animi deleniti laborum modi mollitia repudiandae sint soluta temporibus tenetur?</p>
                        <p class="chat-content-msg__item--time">10:30 10.09</p>
                      </div>
                      <div class="chat-content-msg__item">
                        <img class="chat-content-msg__item--img" src="https://picsum.photos/400/400?image=99" alt="">
                        <p class="chat-content-msg__item--text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium alias animi deleniti laborum modi mollitia repudiandae sint soluta temporibus tenetur?</p>
                        <p class="chat-content-msg__item--time">10:30 10.09</p>
                      </div>
                      <div class="chat-content-msg__item">
                        <img class="chat-content-msg__item--img" src="https://picsum.photos/400/400?image=87" alt="">
                        <p class="chat-content-msg__item--text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium alias animi deleniti laborum modi mollitia repudiandae sint soluta temporibus tenetur?</p>
                        <p class="chat-content-msg__item--time">10:30 10.09</p>
                      </div>
                      <div class="chat-content-msg__item ownMsg">
                        <img class="chat-content-msg__item--img" src="https://picsum.photos/400/400?image=70" alt="">
                        <p class="chat-content-msg__item--text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium alias animi deleniti laborum modi mollitia repudiandae sint soluta temporibus tenetur?</p>
                        <p class="chat-content-msg__item--time">10:30 10.09</p>
                      </div>
                      <div class="chat-content-msg__item ownMsg">
                        <img class="chat-content-msg__item--img" src="https://picsum.photos/400/400?image=43" alt="">
                        <p class="chat-content-msg__item--text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium alias animi deleniti laborum modi mollitia repudiandae sint soluta temporibus tenetur?</p>
                        <p class="chat-content-msg__item--time">10:30 10.09</p>
                      </div>
                      <div class="chat-content-msg__item ">
                        <img class="chat-content-msg__item--img" src="https://picsum.photos/400/400?image=33" alt="">
                        <p class="chat-content-msg__item--text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium alias animi deleniti laborum modi mollitia repudiandae sint soluta temporibus tenetur?</p>
                        <p class="chat-content-msg__item--time">10:30 10.09</p>
                      </div>
                    </div>

                    <div class="chat-send-msg">
                      <!--                     <vs-input style="flex-basis: 75%" size="large" placeholder="msg" v-model="value1" />-->
                      <vs-textarea  style="flex-basis: 75%; margin-bottom: 0" label="Yor message"  />
                      <vs-button   color="#28DEEF" type="filled" >
                        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                          <path d="M3 8C3 8.55 3.45 9 4 9C4.55 9 5 8.55 5 8V6H7C7.55 6 8 5.55 8 5C8 4.45 7.55 4 7 4H5V2C5 1.45 4.55 1 4 1C3.45 1 3 1.45 3 2V4H1C0.45 4 0 4.45 0 5C0 5.55 0.45 6 1 6H3V8Z" fill="white"/>
                          <path d="M13 17C14.6569 17 16 15.6569 16 14C16 12.3431 14.6569 11 13 11C11.3431 11 10 12.3431 10 14C10 15.6569 11.3431 17 13 17Z" fill="white"/>
                          <path d="M21 6H17.83L16.59 4.65C16.4036 4.44539 16.1767 4.28191 15.9235 4.16999C15.6704 4.05807 15.3968 4.00017 15.12 4H8.72C8.89 4.3 9 4.63 9 5C9 6.1 8.1 7 7 7H6V8C6 9.1 5.1 10 4 10C3.63 10 3.3 9.89 3 9.72V20C3 21.1 3.9 22 5 22H21C22.1 22 23 21.1 23 20V8C23 6.9 22.1 6 21 6ZM13 19C10.24 19 8 16.76 8 14C8 11.24 10.24 9 13 9C15.76 9 18 11.24 18 14C18 16.76 15.76 19 13 19Z" fill="white"/>
                        </svg>
                      </vs-button>
                      <vs-button   color="#5753E8" type="filled" ><svg width="24" height="24" viewBox="0 0 30 30" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M29.7426 0.257471C29.494 0.00879953 29.121 -0.0676652 28.7947 0.0628814L0.55251 11.3596C0.229366 11.4889 0.0129796 11.7966 0.000557715 12.1445C-0.0118055 12.4923 0.182257 12.8146 0.495381 12.9665L11.6322 18.3677L17.0334 29.5045C17.1807 29.8082 17.4884 29.9999 17.824 29.9999C17.8345 29.9999 17.845 29.9997 17.8555 29.9993C18.2032 29.9869 18.5111 29.7706 18.6403 29.4474L29.9371 1.2054C30.0677 0.878915 29.9912 0.506084 29.7426 0.257471ZM3.05235 12.2529L25.4718 3.28524L12.1108 16.6462L3.05235 12.2529ZM17.747 26.9476L13.3537 17.8891L26.7148 4.52813L17.747 26.9476Z" fill="white"/>
                      </svg>
                      </vs-button>


                    </div>

                  </div>
                </div>
              </div>
            </div>
          </transition>
          <transition name = "fade">
            <div v-show="activeTab==='userVip'" class="profile-right">
              <div class="block-rounded p20 profile-balance">
                <img src="/profile-balance-icon.png" alt="">
                <p class="profile-balance__amount text-blue">2350</p>
                <p class="profile-balance__text">我的余额</p>

                <div class="btn btn-outline btn-outline-blue">
                  <div class="btn-outline-inner">
                    <p>
                      申请申请
                    </p>
                  </div>
                </div>
                <div class="btn btn-blue btn-round">
                  <p>申请</p>
                </div>


              </div>
              <img src="/p-vip_img-1.png" alt="">
              <img src="/p-vip_img-2.png" alt="">
              <img src="/p-vip_img-3.png" alt="">
              <img src="/p-vip_img-4.png" alt="">
              <img src="/p-vip_img-5.png" alt="">
            </div>
          </transition>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
  export default {
    data(){
      return {
        value1:'',
        value2:'',
        value3:'',
        activeTab:'userInfo'
      }
    }
  }
</script>


<style>
  .con-upload {
    width: unset !important;
  }
  .con-input-upload {
    margin: 0 !important;
    width: 100px !important;
    height: 100px !important;
  }
  .con-input-upload .text-input {
    font-size: 13px !important;
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
