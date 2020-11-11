<template>
  <div>
    <section class="profile">
      <div class="container">
        <div class="profile-user-area">
          <div class="profile-user-area__img" style="background: url(/test_profile_m_bg.png) no-repeat center"></div>
          <div class="profile-user-area__avatar">
            <img src="https://media.gettyimages.com/photos/portrait-of-a-young-malay-man-in-a-modern-office-picture-id1178688517?s=2048x2048" alt="">
          </div>
          <div class="profile-user-area__info">
            <div class="profile-user-area__info--name">
              <p>li pin hin</p>
              <p><a href="#">@promoman</a></p>
            </div>
            <div class="profile-user-area__info--buttons">
              <div class="btn btn-d-blue-solid btn-hover-shadow"><p>写一条消息</p></div>

              <div class="btn btn-l-blue-solid btn-hover-shadow"><p>找出联络人</p></div>
            </div>
          </div>
        </div>
        <div class="profile-wrapper">
          <div class="profile-left">
            <div @click="activeTab='userVip'" class="block-rounded p20 profile-balance">
              <div class="profile-balance__group">
                <img src="/profile-balance-icon.png" alt="">
                <div class="">
                   <p class="profile-balance__amount ">2350</p>
                <p class="profile-balance__text">我的余额</p>
                </div>

              </div>

              <div class="profile-balance__group">
                <div style="margin-right: 10px" class="btn btn-grey-outline">

                  <span>补充</span>
                </div>
                <div class="btn btn-grey-outline">

                  <span>如何使用</span>
                </div>
              </div>

            </div>
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
                <li class="profile-menu__item ">
                  <svg width="32" height="28" viewBox="0 0 32 28" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M3.34138 9.21389L5.25474 25.0953H26.7451L28.6584 9.21389L22.6922 13.096L15.9999 3.95058L9.30761 13.096L3.34138 9.21389ZM2.31328 5.05291L8.56071 9.11948L14.7888 0.60873C14.9264 0.420461 15.1081 0.267 15.3188 0.16112C15.5294 0.0552389 15.763 0 15.9999 0C16.2368 0 16.4704 0.0552389 16.681 0.16112C16.8917 0.267 17.0734 0.420461 17.211 0.60873L23.4391 9.11948L29.688 5.05291C29.9245 4.89932 30.2011 4.81503 30.4851 4.80999C30.7691 4.80495 31.0487 4.87938 31.2907 5.02448C31.5328 5.16958 31.7273 5.37929 31.8511 5.62882C31.975 5.87835 32.0231 6.15728 31.9897 6.43264L29.5452 26.7176C29.5026 27.0709 29.3286 27.3966 29.0562 27.633C28.7839 27.8694 28.4322 28 28.0678 28H3.93205C3.56763 28 3.2159 27.8694 2.94357 27.633C2.67124 27.3966 2.49726 27.0709 2.45462 26.7176L0.0101049 6.43119C-0.0229251 6.15595 0.0254075 5.87722 0.149397 5.62792C0.273387 5.37862 0.467857 5.16915 0.709852 5.02424C0.951846 4.87933 1.23126 4.80503 1.51511 4.81011C1.79896 4.81519 2.0754 4.89944 2.31179 5.05291H2.31328ZM15.9999 19.2859C15.2107 19.2859 14.4538 18.9799 13.8958 18.4352C13.3377 17.8904 13.0242 17.1516 13.0242 16.3812C13.0242 15.6108 13.3377 14.872 13.8958 14.3273C14.4538 13.7826 15.2107 13.4765 15.9999 13.4765C16.7891 13.4765 17.546 13.7826 18.104 14.3273C18.6621 14.872 18.9756 15.6108 18.9756 16.3812C18.9756 17.1516 18.6621 17.8904 18.104 18.4352C17.546 18.9799 16.7891 19.2859 15.9999 19.2859Z" fill="url(#paint0_linear)"/>
                    <defs>
                      <linearGradient id="paint0_linear" x1="-0.248962" y1="-5.44702e-06" x2="34.6143" y2="3.91731" gradientUnits="userSpaceOnUse">
                        <stop stop-color="#EF422B"/>
                        <stop offset="1" stop-color="#EFDB28"/>
                      </linearGradient>
                    </defs>
                  </svg>
                  <p class="text-orange fs-22">
                    VIP功能
                  </p>
                </li>
              </ul>
            </div>
            <!--            <div class="btn btn-orange btn-w-img">-->
            <!--              <svg width="26" height="26" viewBox="0 0 32 28" fill="none" xmlns="http://www.w3.org/2000/svg">-->
            <!--                <path d="M3.34138 9.21389L5.25474 25.0953H26.7451L28.6584 9.21389L22.6922 13.096L15.9999 3.95058L9.30761 13.096L3.34138 9.21389ZM2.31328 5.05291L8.56071 9.11948L14.7888 0.60873C14.9264 0.420461 15.1081 0.267 15.3188 0.16112C15.5294 0.0552389 15.763 0 15.9999 0C16.2368 0 16.4704 0.0552389 16.681 0.16112C16.8917 0.267 17.0734 0.420461 17.211 0.60873L23.4391 9.11948L29.688 5.05291C29.9245 4.89932 30.2011 4.81503 30.4851 4.80999C30.7691 4.80495 31.0487 4.87938 31.2907 5.02448C31.5328 5.16958 31.7273 5.37929 31.8511 5.62882C31.975 5.87835 32.0231 6.15728 31.9897 6.43264L29.5452 26.7176C29.5026 27.0709 29.3286 27.3966 29.0562 27.633C28.7839 27.8694 28.4322 28 28.0678 28H3.93205C3.56763 28 3.2159 27.8694 2.94357 27.633C2.67124 27.3966 2.49726 27.0709 2.45462 26.7176L0.0101049 6.43119C-0.0229251 6.15595 0.0254075 5.87722 0.149397 5.62792C0.273387 5.37862 0.467857 5.16915 0.709852 5.02424C0.951846 4.87933 1.23126 4.80503 1.51511 4.81011C1.79896 4.81519 2.0754 4.89944 2.31179 5.05291H2.31328ZM15.9999 19.2859C15.2107 19.2859 14.4538 18.9799 13.8958 18.4352C13.3377 17.8904 13.0242 17.1516 13.0242 16.3812C13.0242 15.6108 13.3377 14.872 13.8958 14.3273C14.4538 13.7826 15.2107 13.4765 15.9999 13.4765C16.7891 13.4765 17.546 13.7826 18.104 14.3273C18.6621 14.872 18.9756 15.6108 18.9756 16.3812C18.9756 17.1516 18.6621 17.8904 18.104 18.4352C17.546 18.9799 16.7891 19.2859 15.9999 19.2859Z" fill="white"/>-->
            <!--              </svg>-->
            <!--              <p>-->
            <!--                VIP 我的简历-->
            <!--              </p>-->
            <!--            </div>-->
          </div>

          <div v-show="activeTab==='userInfo'" class="profile-right">

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


          <div v-show="activeTab==='userFriends'" class="profile-right">

            <div class="models-wrapper">

              <div class="model-item">
                <nuxt-link to="/girl-profile">
                  <div class="model-item__bg" style="background: url(/test_bg.png)"></div>
                  <div class="model-item__img">
                    <img src="https://media.gettyimages.com/photos/teenage-beauty-picture-id1126913832?s=2048x2048" alt="">
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
                    <img src="https://media.gettyimages.com/photos/beautiful-woman-soft-makeup-and-perfect-skin-picture-id1133213198?s=2048x2048" alt="">
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
                    <img src="https://media.gettyimages.com/photos/beautiful-woman-picture-id1138676758?s=2048x2048" alt="">
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


          <div v-show="activeTab==='userFavorites'" class="profile-right">

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
                  <div class="group-item__top" style="background: url(https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcR_Ft1YaZT4eIP7SDW-1ETwdUgL2FOi0RkdaA&usqp=CAU)"></div>
                  <div class="group-item__button">
                    <img draggable="false" src="/group_icon.png" alt="">
                  </div>
                  <div class="group-item__img">
                    <img draggable="false" src="https://www.iconarchive.com/download/i1878/3xhumed/mega-games-pack-39/Call-of-Duty-World-at-War-10.ico" alt="">
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
                  <div class="group-item__top" style="background: url(data:image/jpeg;base64,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)"></div>
                  <div class="group-item__button">
                    <img draggable="false" src="/group_icon.png" alt="">
                  </div>
                  <div class="group-item__img">
                    <img draggable="false" src="data:image/jpeg;base64,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" alt="">
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


          <div v-show="activeTab==='userSettings'" class="profile-right">

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

          <div v-show="activeTab==='userChat'" class="profile-right">

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


          <div v-show="activeTab==='userVip'" class="profile-right">

            <img src="/p-vip_img-1.png" alt="">
            <img src="/p-vip_img-2.png" alt="">
            <img src="/p-vip_img-3.png" alt="">
            <img src="/p-vip_img-4.png" alt="">
            <img src="/p-vip_img-5.png" alt="">
          </div>

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
