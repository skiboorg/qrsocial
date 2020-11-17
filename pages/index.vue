<template>
  <div>
    <div class="page-fixed">

      <div class="page-fixed__info-btn">
        <p @click="infoModal=true">
          <svg width="38" height="38" viewBox="0 0 38 38" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M19 37.3332C8.87446 37.3332 0.666626 29.1253 0.666626 18.9998C0.666626 8.87434 8.87446 0.666504 19 0.666504C29.1255 0.666504 37.3333 8.87434 37.3333 18.9998C37.3333 29.1253 29.1255 37.3332 19 37.3332ZM19 33.6665C22.8898 33.6665 26.6203 32.1213 29.3709 29.3707C32.1214 26.6202 33.6666 22.8897 33.6666 18.9998C33.6666 15.11 32.1214 11.3795 29.3709 8.62894C26.6203 5.8784 22.8898 4.33317 19 4.33317C15.1101 4.33317 11.3796 5.8784 8.62906 8.62894C5.87853 11.3795 4.33329 15.11 4.33329 18.9998C4.33329 22.8897 5.87853 26.6202 8.62906 29.3707C11.3796 32.1213 15.1101 33.6665 19 33.6665ZM19 15.3332C19.4862 15.3332 19.9525 15.5263 20.2963 15.8701C20.6401 16.214 20.8333 16.6803 20.8333 17.1665V26.3332C20.8333 26.8194 20.6401 27.2857 20.2963 27.6295C19.9525 27.9734 19.4862 28.1665 19 28.1665C18.5137 28.1665 18.0474 27.9734 17.7036 27.6295C17.3598 27.2857 17.1666 26.8194 17.1666 26.3332V17.1665C17.1666 16.6803 17.3598 16.214 17.7036 15.8701C18.0474 15.5263 18.5137 15.3332 19 15.3332ZM19 13.4998C18.5137 13.4998 18.0474 13.3067 17.7036 12.9629C17.3598 12.6191 17.1666 12.1527 17.1666 11.6665C17.1666 11.1803 17.3598 10.714 17.7036 10.3701C18.0474 10.0263 18.5137 9.83317 19 9.83317C19.4862 9.83317 19.9525 10.0263 20.2963 10.3701C20.6401 10.714 20.8333 11.1803 20.8333 11.6665C20.8333 12.1527 20.6401 12.6191 20.2963 12.9629C19.9525 13.3067 19.4862 13.4998 19 13.4998Z" fill="#3E3F5E"/>
          </svg>
          <span>关于我们</span>
        </p>

          <p>
            <svg width="40" height="40" viewBox="0 0 40 40" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M17.5052 27.5C17.5052 27.1717 17.5699 26.8466 17.6955 26.5433C17.8211 26.24 18.0053 25.9644 18.2374 25.7322C18.4696 25.5001 18.7452 25.3159 19.0485 25.1903C19.3518 25.0647 19.6769 25 20.0052 25C20.3335 25 20.6586 25.0647 20.9619 25.1903C21.2652 25.3159 21.5408 25.5001 21.773 25.7322C22.0051 25.9644 22.1893 26.24 22.3149 26.5433C22.4405 26.8466 22.5052 27.1717 22.5052 27.5C22.5052 28.163 22.2418 28.7989 21.773 29.2678C21.3041 29.7366 20.6682 30 20.0052 30C19.3422 30 18.7063 29.7366 18.2374 29.2678C17.7686 28.7989 17.5052 28.163 17.5052 27.5V27.5ZM20.1252 24C20.9652 24 21.3852 23.4 21.5102 22.4325C21.6102 21.0975 22.0052 20.395 23.6277 19.2825C25.3102 18.095 26.2502 16.5575 26.2502 14.3175C26.2502 11.005 23.9502 8.75 20.5952 8.75C18.0452 8.75 16.1152 9.98 15.3452 11.975C15.1119 12.5199 14.9944 13.1073 15.0002 13.7C15.0002 14.6825 15.5077 15.3 16.3627 15.3C17.0427 15.3 17.5002 14.9325 17.7727 14.025C18.1677 12.545 19.0852 11.7375 20.4577 11.7375C21.9827 11.7375 23.0327 12.8525 23.0327 14.4475C23.0327 15.855 22.5127 16.66 20.9777 17.76C19.4302 18.8425 18.6627 20.045 18.6627 21.86V22.1375C18.6627 23.2075 19.1827 24 20.1252 24Z" fill="#585858"/>
              <path fill-rule="evenodd" clip-rule="evenodd" d="M25.6813 6.28049L23.3788 3.92049L25.1663 2.17549L26.7213 3.76799L28.9463 3.74049C29.9095 3.72909 30.8651 3.91038 31.7572 4.27371C32.6492 4.63703 33.4596 5.17506 34.1407 5.85614C34.8218 6.53722 35.3598 7.3476 35.7231 8.23964C36.0864 9.13168 36.2677 10.0874 36.2563 11.0505L36.2313 13.2755L37.8213 14.8305C38.51 15.5034 39.0572 16.3072 39.4308 17.1946C39.8044 18.082 39.9968 19.0351 39.9968 19.998C39.9968 20.9608 39.8044 21.914 39.4308 22.8014C39.0572 23.6888 38.51 24.4926 37.8213 25.1655L36.2288 26.7205L36.2563 28.9455C36.2677 29.9086 36.0864 30.8643 35.7231 31.7563C35.3598 32.6484 34.8218 33.4588 34.1407 34.1398C33.4596 34.8209 32.6492 35.3589 31.7572 35.7223C30.8651 36.0856 29.9095 36.2669 28.9463 36.2555L26.7213 36.2305L25.1663 37.8205C24.4934 38.5091 23.6896 39.0563 22.8022 39.4299C21.9148 39.8035 20.9617 39.996 19.9988 39.996C19.036 39.996 18.0829 39.8035 17.1955 39.4299C16.3081 39.0563 15.5043 38.5091 14.8313 37.8205L13.2763 36.228L11.0513 36.2555C10.0882 36.2669 9.13254 36.0856 8.2405 35.7223C7.34846 35.3589 6.53807 34.8209 5.85699 34.1398C5.17591 33.4588 4.63789 32.6484 4.27456 31.7563C3.91124 30.8643 3.72994 29.9086 3.74134 28.9455L3.76634 26.7205L2.17634 25.1655C1.48769 24.4926 0.940494 23.6888 0.5669 22.8014C0.193306 21.914 0.000854492 20.9608 0.000854492 19.998C0.000854492 19.0351 0.193306 18.082 0.5669 17.1946C0.940494 16.3072 1.48769 15.5034 2.17634 14.8305L3.76884 13.2755L3.74134 11.0505C3.72994 10.0874 3.91124 9.13168 4.27456 8.23964C4.63789 7.3476 5.17591 6.53722 5.85699 5.85614C6.53807 5.17506 7.34846 4.63703 8.2405 4.27371C9.13254 3.91038 10.0882 3.72909 11.0513 3.74049L13.2763 3.76549L14.8313 2.17549C15.5043 1.48684 16.3081 0.93964 17.1955 0.566046C18.0829 0.192452 19.036 0 19.9988 0C20.9617 0 21.9148 0.192452 22.8022 0.566046C23.6896 0.93964 24.4934 1.48684 25.1663 2.17549L23.3788 3.92049C22.9387 3.46995 22.413 3.11195 21.8326 2.86753C21.2521 2.6231 20.6287 2.49719 19.9988 2.49719C19.369 2.49719 18.7456 2.6231 18.1651 2.86753C17.5847 3.11195 17.0589 3.46995 16.6188 3.92049L14.3188 6.28049L11.0188 6.24049C10.3893 6.23345 9.76467 6.3523 9.1817 6.59006C8.59872 6.82781 8.06914 7.17968 7.62407 7.62499C7.17899 8.07029 6.8274 8.60006 6.58995 9.18316C6.3525 9.76626 6.23397 10.3909 6.24134 11.0205L6.28134 14.3155L3.92134 16.618C3.47081 17.0581 3.11281 17.5838 2.86838 18.1643C2.62396 18.7447 2.49804 19.3682 2.49804 19.998C2.49804 20.6278 2.62396 21.2513 2.86838 21.8317C3.11281 22.4122 3.47081 22.9379 3.92134 23.378L6.28134 25.678L6.24134 28.978C6.2343 29.6075 6.35315 30.2322 6.59091 30.8151C6.82867 31.3981 7.18053 31.9277 7.62584 32.3728C8.07115 32.8178 8.60091 33.1694 9.18402 33.4069C9.76712 33.6443 10.3918 33.7629 11.0213 33.7555L14.3163 33.7155L16.6188 36.0755C17.0589 36.526 17.5847 36.884 18.1651 37.1284C18.7456 37.3729 19.369 37.4988 19.9988 37.4988C20.6287 37.4988 21.2521 37.3729 21.8326 37.1284C22.413 36.884 22.9387 36.526 23.3788 36.0755L25.6788 33.7155L28.9788 33.7555C29.6084 33.7625 30.233 33.6437 30.816 33.4059C31.399 33.1682 31.9285 32.8163 32.3736 32.371C32.8187 31.9257 33.1703 31.3959 33.4077 30.8128C33.6452 30.2297 33.7637 29.605 33.7563 28.9755L33.7163 25.6805L36.0763 23.378C36.5269 22.9379 36.8849 22.4122 37.1293 21.8317C37.3737 21.2513 37.4996 20.6278 37.4996 19.998C37.4996 19.3682 37.3737 18.7447 37.1293 18.1643C36.8849 17.5838 36.5269 17.0581 36.0763 16.618L33.7163 14.318L33.7563 11.018C33.7634 10.3884 33.6445 9.76382 33.4068 9.18084C33.169 8.59787 32.8172 8.06829 32.3718 7.62321C31.9265 7.17814 31.3968 6.82655 30.8137 6.58909C30.2306 6.35164 29.6059 6.23312 28.9763 6.24049L25.6813 6.28049V6.28049Z" fill="#585858"/>
            </svg>
            <span>关于我们</span>
          </p>
                 <p>
           <svg width="40" height="40" viewBox="0 0 40 40" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M13.3333 34.9993H6.66663C6.2246 34.9993 5.80067 34.8238 5.48811 34.5112C5.17555 34.1986 4.99996 33.7747 4.99996 33.3327V26.666C4.99996 26.224 4.82436 25.8001 4.5118 25.4875C4.19924 25.1749 3.77532 24.9993 3.33329 24.9993C2.89126 24.9993 2.46734 25.1749 2.15478 25.4875C1.84222 25.8001 1.66663 26.224 1.66663 26.666V33.3327C1.66663 34.6588 2.19341 35.9305 3.13109 36.8682C4.06877 37.8059 5.34054 38.3327 6.66663 38.3327H13.3333C13.7753 38.3327 14.1992 38.1571 14.5118 37.8445C14.8244 37.532 15 37.108 15 36.666C15 36.224 14.8244 35.8001 14.5118 35.4875C14.1992 35.1749 13.7753 34.9993 13.3333 34.9993V34.9993ZM36.6666 24.9993C36.2246 24.9993 35.8007 25.1749 35.4881 25.4875C35.1755 25.8001 35 26.224 35 26.666V33.3327C35 33.7747 34.8244 34.1986 34.5118 34.5112C34.1992 34.8238 33.7753 34.9993 33.3333 34.9993H26.6666C26.2246 34.9993 25.8007 35.1749 25.4881 35.4875C25.1756 35.8001 25 36.224 25 36.666C25 37.108 25.1756 37.532 25.4881 37.8445C25.8007 38.1571 26.2246 38.3327 26.6666 38.3327H33.3333C34.6594 38.3327 35.9311 37.8059 36.8688 36.8682C37.8065 35.9305 38.3333 34.6588 38.3333 33.3327V26.666C38.3333 26.224 38.1577 25.8001 37.8451 25.4875C37.5326 25.1749 37.1086 24.9993 36.6666 24.9993ZM33.3333 1.66602H26.6666C26.2246 1.66602 25.8007 1.84161 25.4881 2.15417C25.1756 2.46673 25 2.89065 25 3.33268C25 3.77471 25.1756 4.19863 25.4881 4.51119C25.8007 4.82375 26.2246 4.99935 26.6666 4.99935H33.3333C33.7753 4.99935 34.1992 5.17494 34.5118 5.4875C34.8244 5.80006 35 6.22399 35 6.66602V13.3327C35 13.7747 35.1755 14.1986 35.4881 14.5112C35.8007 14.8238 36.2246 14.9993 36.6666 14.9993C37.1086 14.9993 37.5326 14.8238 37.8451 14.5112C38.1577 14.1986 38.3333 13.7747 38.3333 13.3327V6.66602C38.3333 5.33993 37.8065 4.06816 36.8688 3.13048C35.9311 2.1928 34.6594 1.66602 33.3333 1.66602V1.66602ZM3.33329 14.9993C3.77532 14.9993 4.19924 14.8238 4.5118 14.5112C4.82436 14.1986 4.99996 13.7747 4.99996 13.3327V6.66602C4.99996 6.22399 5.17555 5.80006 5.48811 5.4875C5.80067 5.17494 6.2246 4.99935 6.66663 4.99935H13.3333C13.7753 4.99935 14.1992 4.82375 14.5118 4.51119C14.8244 4.19863 15 3.77471 15 3.33268C15 2.89065 14.8244 2.46673 14.5118 2.15417C14.1992 1.84161 13.7753 1.66602 13.3333 1.66602H6.66663C5.34054 1.66602 4.06877 2.1928 3.13109 3.13048C2.19341 4.06816 1.66663 5.33993 1.66663 6.66602V13.3327C1.66663 13.7747 1.84222 14.1986 2.15478 14.5112C2.46734 14.8238 2.89126 14.9993 3.33329 14.9993ZM16.6666 8.33268H9.99996C9.55793 8.33268 9.13401 8.50828 8.82145 8.82084C8.50889 9.1334 8.33329 9.55732 8.33329 9.99935V16.666C8.33329 17.108 8.50889 17.532 8.82145 17.8445C9.13401 18.1571 9.55793 18.3327 9.99996 18.3327H16.6666C17.1087 18.3327 17.5326 18.1571 17.8451 17.8445C18.1577 17.532 18.3333 17.108 18.3333 16.666V9.99935C18.3333 9.55732 18.1577 9.1334 17.8451 8.82084C17.5326 8.50828 17.1087 8.33268 16.6666 8.33268ZM15 14.9993H11.6666V11.666H15V14.9993ZM23.3333 18.3327H30C30.442 18.3327 30.8659 18.1571 31.1785 17.8445C31.491 17.532 31.6666 17.108 31.6666 16.666V9.99935C31.6666 9.55732 31.491 9.1334 31.1785 8.82084C30.8659 8.50828 30.442 8.33268 30 8.33268H23.3333C22.8913 8.33268 22.4673 8.50828 22.1548 8.82084C21.8422 9.1334 21.6666 9.55732 21.6666 9.99935V16.666C21.6666 17.108 21.8422 17.532 22.1548 17.8445C22.4673 18.1571 22.8913 18.3327 23.3333 18.3327ZM25 11.666H28.3333V14.9993H25V11.666ZM16.6666 21.666H9.99996C9.55793 21.666 9.13401 21.8416 8.82145 22.1542C8.50889 22.4667 8.33329 22.8907 8.33329 23.3327V29.9993C8.33329 30.4414 8.50889 30.8653 8.82145 31.1779C9.13401 31.4904 9.55793 31.666 9.99996 31.666H16.6666C17.1087 31.666 17.5326 31.4904 17.8451 31.1779C18.1577 30.8653 18.3333 30.4414 18.3333 29.9993V23.3327C18.3333 22.8907 18.1577 22.4667 17.8451 22.1542C17.5326 21.8416 17.1087 21.666 16.6666 21.666ZM15 28.3327H11.6666V24.9993H15V28.3327ZM23.3333 26.666C23.7753 26.666 24.1992 26.4904 24.5118 26.1779C24.8244 25.8653 25 25.4414 25 24.9993C25.442 24.9993 25.8659 24.8238 26.1785 24.5112C26.491 24.1986 26.6666 23.7747 26.6666 23.3327C26.6666 22.8907 26.491 22.4667 26.1785 22.1542C25.8659 21.8416 25.442 21.666 25 21.666H23.3333C22.8913 21.666 22.4673 21.8416 22.1548 22.1542C21.8422 22.4667 21.6666 22.8907 21.6666 23.3327V24.9993C21.6666 25.4414 21.8422 25.8653 22.1548 26.1779C22.4673 26.4904 22.8913 26.666 23.3333 26.666ZM30 21.666C29.5579 21.666 29.134 21.8416 28.8214 22.1542C28.5089 22.4667 28.3333 22.8907 28.3333 23.3327V28.3327C27.8913 28.3327 27.4673 28.5083 27.1548 28.8208C26.8422 29.1334 26.6666 29.5573 26.6666 29.9993C26.6666 30.4414 26.8422 30.8653 27.1548 31.1779C27.4673 31.4904 27.8913 31.666 28.3333 31.666H30C30.442 31.666 30.8659 31.4904 31.1785 31.1779C31.491 30.8653 31.6666 30.4414 31.6666 29.9993V23.3327C31.6666 22.8907 31.491 22.4667 31.1785 22.1542C30.8659 21.8416 30.442 21.666 30 21.666ZM23.3333 28.3327C23.0037 28.3327 22.6814 28.4304 22.4073 28.6136C22.1333 28.7967 21.9196 29.057 21.7935 29.3615C21.6673 29.6661 21.6343 30.0012 21.6986 30.3245C21.763 30.6478 21.9217 30.9448 22.1548 31.1779C22.3879 31.4109 22.6848 31.5697 23.0081 31.634C23.3314 31.6983 23.6666 31.6653 23.9711 31.5391C24.2756 31.413 24.5359 31.1994 24.7191 30.9253C24.9022 30.6512 25 30.329 25 29.9993C25 29.5573 24.8244 29.1334 24.5118 28.8208C24.1992 28.5083 23.7753 28.3327 23.3333 28.3327Z" fill="#585858"/>
</svg>

            <span>关于我们</span>
          </p>

      </div>
      <a href="#top">
        <div  class="page-fixed__top-btn">
          <svg width="27" height="27" viewBox="0 0 27 27" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M26.3633 14.7104L14.3708 0.889623C14.2624 0.764563 14.1284 0.664265 13.9778 0.595526C13.8273 0.526786 13.6637 0.491211 13.4982 0.491211C13.3327 0.491211 13.1691 0.526786 13.0186 0.595526C12.868 0.664265 12.734 0.764563 12.6256 0.889623L0.636717 14.7104C0.600489 14.7521 0.576999 14.8033 0.569045 14.8579C0.561091 14.9125 0.569008 14.9683 0.591853 15.0186C0.614698 15.0688 0.651508 15.1115 0.697899 15.1414C0.74429 15.1713 0.798307 15.1873 0.853514 15.1874H3.78027C3.94648 15.1874 4.10547 15.1151 4.21748 14.9886L12.127 5.87234V26.2187C12.127 26.3777 12.257 26.5078 12.416 26.5078H14.584C14.743 26.5078 14.873 26.3777 14.873 26.2187V5.87234L22.7825 14.9886C22.8909 15.1151 23.0499 15.1874 23.2197 15.1874H26.1465C26.3922 15.1874 26.5259 14.8983 26.3633 14.7104Z" fill="#3E3F5E"/>
          </svg>
        </div>
      </a>
    </div>
    <section id="top" class="banner">
      <!--      <div class="banner-girl-login">-->
      <!--        <p><nuxt-link to="/girl-login">вход для девушек</nuxt-link></p>-->
      <!--      </div>-->
      <!--      <div class="banner-info-label " :class="{'infoBlockActive':showSideBlock}" @click="showSideBlock ? showSideBlock = false : showSideBlock = true">-->
      <!--        <svg width="15" height="53" viewBox="0 0 15 53" fill="none" xmlns="http://www.w3.org/2000/svg">-->
      <!--          <path d="M13.9722 17.7554L0.804724 19.4056L0.333225 21.5906L2.92072 22.0679C4.61123 22.4704 4.94473 23.0799 4.57673 24.7646L0.333225 44.7056C-0.782275 49.8634 0.936976 52.2899 4.97923 52.2899C8.11298 52.2899 11.7527 50.8409 13.403 48.8514L13.909 46.4594C12.759 47.4714 11.08 47.8739 9.96447 47.8739C8.38322 47.8739 7.80823 46.7641 8.21648 44.8091L13.9722 17.7554Z" fill="white"/>-->
      <!--          <path d="M8.625 11.5C11.8006 11.5 14.375 8.92564 14.375 5.75C14.375 2.57436 11.8006 0 8.625 0C5.44936 0 2.875 2.57436 2.875 5.75C2.875 8.92564 5.44936 11.5 8.625 11.5Z" fill="white"/>-->
      <!--        </svg>-->
      <!--        <p>213</p>-->
      <!--      </div>-->
      <!--      <div class="banner-info-block">-->
      <!--        <div class="banner-info-block__top">-->

      <!--            <img class="banner-info-block__top&#45;&#45;img" src="/lip.webp" alt="">-->

      <!--          <div class="banner-info-block__top&#45;&#45;name">-->
      <!--            <p>Li pin hin</p>-->
      <!--            <p>creator QR SOCIAL</p>-->
      <!--          </div>-->
      <!--        </div>-->
      <!--        <div class="banner-info-block__content">-->
      <!--         <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusamus ad culpa enim et, illo modi porro quod similique tempora velit. Ad aut consectetur corporis doloremque enim est eum, iusto modi optio placeat provident quaerat quia repellendus reprehenderit sint veniam voluptatum!</p>-->
      <!--        </div>-->
      <!--      </div>-->
    </section>
    <p class="section-header style-simple text-center mb-60">您将在我们<span>的平台</span>上获得什么？</p>
    <section class="features">
      <div class="container">
        <div class="features-big-wrapper">
          <img src="/feature-img-1.png" alt="">
          <div class="features-text-item">
            <p class="features-text-item__title">与俄罗斯姑娘交流24/7</p>
            <p class="features-text-item__text">与女孩见面并交流：全天候私人聊天或社交团体中！ 交流您的思想和心情，帮助俄罗斯姑娘学习有趣的汉语和迷人的中国文化！</p>
          </div>

          <div class="features-text-item">
            <p class="features-text-item__title">参加视频广播</p>
            <p class="features-text-item__text">参与开发：我们的女孩不断为您播报各种主题！<br>
              共同学习中国语言和文化<br>
              棋盘游戏或电脑游戏<br>
              做运动和瑜伽<br>
              各种爱好：烹饪，绘画或卡拉OK</p>
          </div>
          <img src="/features-img-4.png" alt="">
          <img src="/features-img-2.png" alt="">
          <div class="features-text-item">
            <p class="features-text-item__title">通过评级促进女孩</p>
            <p class="features-text-item__text">评分最高的女孩将前往中国学习和发展文化！ 在那里我们可以与他们见面并在特别会议上现场聊天！<br>
              向女孩们提问，观看广播，赠送礼物并表现出关注的迹象-所有这些都促进了您对评级感兴趣的女孩！</p>
          </div>
          <div class="features-text-item">
            <p class="features-text-item__title">无限的可能性</p>
            <p class="features-text-item__text">我们的平台使用内部货币“水晶”，您可以为此：<br>
              -亲自向女孩购买商品（签名，绘画，带有祝贺和笑话的视频）<br>
              -吸引注意并向选定的女孩赠送礼物和贴纸，同时提升她们的等级<br>
              -为您索取女孩的个人照片<br>
              对于最复杂的平台用户，还有一个VIP帐户：<br>
              私人VIP俱乐部进行交流，可以将照片发送给女孩，进行私人广播和VIP广播，使您的品味：选择广播位置，主题和为女孩打扮的衣服。</p>


          </div>
          <img src="/features-img-3.png" alt="">


        </div>

      </div>
    </section>
    <p style="margin-bottom: 160px" class="section-header style-simple text-center ">您将在我们<span>的平台</span>上获得什么？</p>
    <section class="features-v2">
      <div class="container">
        <div class="features-v2-item align-left">
          <img class="features-v2-item__image pos-left" src="/f-v2-i1.png" alt="">
          <img src="/f-v2-img1.png" alt="">
          <p class="section-subheader mb-10">个人资料</p>
          <p>每个女孩都填写自己的个人资料：她的兴趣，喜欢的电影和音乐类型，书籍和兴趣爱好</p>
        </div>
        <div class="features-v2-item ">
          <img class="features-v2-item__image pos-right" src="/f-v2-i2.png" alt="">
          <img src="/f-v2-img2.png" alt="">
          <p class="section-subheader mb-10">通讯与广播</p>
          <p>女孩为您启动广播并等待响应！ 给她的每条信息，每一份礼物和关注都很重要。 您越活跃，女孩的评价就越高。</p>
        </div>
        <div class="features-v2-item align-left">
          <img class="features-v2-item__image pos-left" src="/f-v2-i3.png" alt="">
          <img src="/f-v2-img3.png" alt="">
          <p class="section-subheader mb-10">学习语言和文化</p>
          <p>在交流过程中，女孩学习汉语和中国文化，学习有关这个美丽国家的信息，并准备搬家</p>
        </div>
        <div class="features-v2-item ">
          <img class="features-v2-item__image pos-right" src="/f-v2-i4.png" alt="">
          <img src="/f-v2-img4.png" alt="">
          <p class="section-subheader mb-10">计算收视率和中国之行</p>
          <p>在六个月的最后，我们将计算出评分最高的女孩，并派她们去中国学习和旅行！ 您将能够与他们见面并聊天，参加常规活动并享有独特的体验！</p>
        </div>
      </div>
    </section>
    <p class="section-header style-simple text-center mb-60">我们的<span>女孩</span>正在等你！</p>
    <section class="models">
      <div class="container">
        <div class="models-wrapper">

          <div class="model-item">
            <nuxt-link to="/girl-profile">
              <div class="model-item__bg" style="background: url(/test_bg.png)"></div>
              <div class="model-item__img">
                <img src="https://media.gettyimages.com/photos/young-beautiful-woman-picture-id1050903354?s=2048x2048" alt="">
              </div>
              <p class="model-item__name">Karina Ivanova</p>
              <p class="model-item__login">@kistochka</p>


            </nuxt-link>
          </div>
          <div class="model-item">
            <nuxt-link to="/girl-profile">
              <div class="model-item__bg" style="background: url(/test_bg.png)"></div>
              <div class="model-item__img">
                <img src="https://media.gettyimages.com/photos/serene-beauty-picture-id1083617440?s=2048x2048" alt="">
              </div>
              <p class="model-item__name">Arina Severnaya</p>
              <p class="model-item__login">@koshka12</p>


            </nuxt-link>
          </div>
          <div class="model-item">
            <nuxt-link to="/girl-profile">
              <div class="model-item__bg" style="background: url(/test_bg.png)"></div>
              <div class="model-item__img">
                <img src="https://media.gettyimages.com/photos/beautiful-woman-picture-id927570754?s=2048x2048" alt="">
              </div>
              <p class="model-item__name">Marianna 女神</p>
              <p class="model-item__login">@mariii</p>


            </nuxt-link>
          </div>


        </div>
      </div>
    </section><!--models-->
    <p class="section-header style-simple text-center mb-60">与女孩<span>预定</span>的广播</p>
    <section class="streams">
      <div class="container">
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
                  <p>在健身房锻炼</p>
                  <p>Karina Ivanova</p>
                </div>
                <div class="stream-item__bottom--right">
                  <img draggable="false" src="https://media.gettyimages.com/photos/young-beautiful-woman-picture-id1050903354?s=2048x2048" alt="">
                </div>
              </div>
            </nuxt-link>
          </div>
          <div class="stream-item ">
            <nuxt-link to="/stream">
              <div class="stream-item__top" style="background: linear-gradient(black, black), url(/s2.png) no-repeat center">
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
                  <p>语言学习</p>
                  <p>Arina Severnaya</p>
                </div>
                <div class="stream-item__bottom--right">
                  <img draggable="false" src="https://media.gettyimages.com/photos/serene-beauty-picture-id1083617440?s=2048x2048" alt="">
                </div>
              </div>
            </nuxt-link>
          </div>
          <div class="stream-item ">
            <nuxt-link to="/stream">
              <div class="stream-item__top" style="background: linear-gradient(black, black), url(/s3.png) no-repeat center">
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
                  <p>烹饪您最喜欢的食物</p>
                  <p>Marianna女神</p>
                </div>
                <div class="stream-item__bottom--right">
                  <img draggable="false" src="https://media.gettyimages.com/photos/beautiful-woman-picture-id927570754?s=2048x2048" alt="">
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
                  <p>VIP捉迷藏游戏</p>
                  <p>Arina Severnaya</p>
                </div>
                <div class="stream-item__bottom--right">
                  <img draggable="false" src="https://media.gettyimages.com/photos/serene-beauty-picture-id1083617440?s=2048x2048" alt="">
                </div>
              </div>
            </nuxt-link>
          </div>
        </div>
      </div>
    </section>
    <p class="section-header style-simple text-center mb-60">我们<span>平台的</span>功能</p>

    <div style="margin-bottom: 150px" class="container">
      <div class="features-small-wrapper">
        <div class="feature-small-item">
          <img draggable="false" src="/feature-small-icon1.png" alt="">
          <p>美丽的俄罗斯姑娘的海洋</p>
        </div>
        <div class="feature-small-item">
          <img draggable="false" src="/feature-small-icon2.png" alt="">
          <p>交流的机会：聊天和广播</p>
        </div>
        <div class="feature-small-item">
          <img draggable="false" src="/feature-small-icon3.png" alt="">
          <p>通过兴趣和爱好互相寻找</p>
        </div>
        <div class="feature-small-item">
          <img draggable="false" src="/feature-small-icon4.png" alt="">
          <p>开放：在个人资料中谈论自己</p>
        </div>

      </div>
    </div>
    <p style="margin-bottom: 120px" class="section-header style-simple text-center ">我们<span>的房</span>价</p>
    <section class="tariff">
      <div class="container">
        <div class="tariff-wrapper">
          <div class="tariff-one">
            <div class="tariff-one__wrapper">
              <p class="tariff-one__name">每月固定费用</p>
              <div class="tariff-one__price">
                <p>每月299元</p>
              </div>
              <div class="tariff-one__info">
                <p class="tariff-one__info-item">+一般聊天中的交流</p>
                <p class="tariff-one__info-item">+使用相机</p>
                <p class="tariff-one__info-item">+送礼物的能力</p>
              </div>
              <div class="btn btn-blue"><p>申请</p></div>
            </div>


          </div>
          <div class="tariff-two">
            <div class="tariff-two__wrapper">
              <p class="tariff-two__name">VIP费是最好的</p>
              <div class="tariff-two__price">
                <p>每月599元</p>
              </div>
              <div class="tariff-two__info">
                <p class="tariff-two__info-item">+一般聊天中的交流</p>
                <p class="tariff-two__info-item">+使用相机</p>
                <p class="tariff-two__info-item">+送礼物的能力</p>
                <p class="tariff-two__info-item">+私人聊天！</p>
                <p class="tariff-two__info-item">+特殊表情</p>
                <p class="tariff-two__info-item">+速度优先</p>
              </div>
              <div class="btn btn-orange"><p>申请</p></div>
            </div>


          </div>
          <div class="tariff-three">
            <div class="tariff-three__wrapper">
              <p class="tariff-three__name">个人关税</p>
              <div class="tariff-three__price">
                <p>每月299元</p>
              </div>
              <div class="tariff-three__info">
                <p class="tariff-three__info-item">+一般聊天中的交流</p>
                <p class="tariff-three__info-item">+使用相机</p>
                <p class="tariff-three__info-item">+送礼物的能力</p>
              </div>
              <div class="btn btn-white"><p>申请</p></div>
            </div>


          </div>
        </div>
      </div>
    </section><!--tariffs-->
    <!--   <p class="section-header style-simple text-center mb-60">我们<span>平台的</span>功能</p>-->

    <!--    <section class="groups">-->
    <!--      <div class="container">-->
    <!--        <div class="groups-wrapper">-->
    <!--          <div class="group-item">-->
    <!--            <nuxt-link to="/group-profile">-->
    <!--              <div class="group-item__top" style="background: url(/test_g_bg.png)"></div>-->
    <!--              <div class="group-item__button">-->
    <!--                <img draggable="false" src="/group_icon.png" alt="">-->
    <!--              </div>-->
    <!--              <div class="group-item__img">-->
    <!--                <img draggable="false" src="https://www.wotcheatmods.com/wp-content/uploads/2020/04/440_wot_premium.png" alt="">-->
    <!--              </div>-->
    <!--              <div class="group-item__title">我们爱坦克世界</div>-->
    <!--              <div class="group-item__subtitle">广播评级广播评级</div>-->
    <!--              <div class="group-item__numbers">-->
    <!--                <div class="group-item__number">-->
    <!--                  <p>120</p>-->
    <!--                  <p>广播的数</p>-->
    <!--                </div>-->
    <!--                <div class="group-item__number">-->
    <!--                  <p>120</p>-->
    <!--                  <p>广播的数</p>-->
    <!--                </div>-->
    <!--                <div class="group-item__number">-->
    <!--                  <p>120</p>-->
    <!--                  <p>广播的数</p>-->
    <!--                </div>-->
    <!--              </div>-->
    <!--              <div class="group-item__avatars">-->
    <!--              <span class="group-item__avatar">-->
    <!--                  <img src="https://www.fillmurray.com/50/50" width="50" height="50"/>-->
    <!--              </span>-->
    <!--                <span class="group-item__avatar">-->
    <!--                  <img src="https://www.fillmurray.com/100/100" width="50" height="50"/>-->
    <!--              </span>-->
    <!--                <span class="group-item__avatar">-->
    <!--                <img src="https://www.fillmurray.com/200/200" width="50" height="50"/>-->
    <!--              </span>-->
    <!--                <span class="group-item__avatar">-->
    <!--                <img src="https://www.fillmurray.com/150/150" width="50" height="50"/>-->
    <!--              </span>-->
    <!--                <span class="group-item__avatar">-->
    <!--                  <img src="https://www.fillmurray.com/50/50" width="50" height="50"/>-->
    <!--              </span>-->
    <!--                <span class="group-item__avatar">-->
    <!--                  <p>+ 12</p>-->
    <!--              </span>-->
    <!--              </div>-->
    <!--              <div class="btn btn-blue-solid"><p>加入小组</p></div>-->
    <!--            </nuxt-link>-->
    <!--          </div>-->
    <!--          <div class="group-item">-->
    <!--            <nuxt-link to="/group-profile">-->
    <!--              <div class="group-item__top" style="background: url(https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcR_Ft1YaZT4eIP7SDW-1ETwdUgL2FOi0RkdaA&usqp=CAU)"></div>-->
    <!--              <div class="group-item__button">-->
    <!--                <img draggable="false" src="/group_icon.png" alt="">-->
    <!--              </div>-->
    <!--              <div class="group-item__img">-->
    <!--                <img draggable="false" src="https://www.iconarchive.com/download/i1878/3xhumed/mega-games-pack-39/Call-of-Duty-World-at-War-10.ico" alt="">-->
    <!--              </div>-->
    <!--              <div class="group-item__title">我们爱坦克世界</div>-->
    <!--              <div class="group-item__subtitle">广播评级广播评级</div>-->
    <!--              <div class="group-item__numbers">-->
    <!--                <div class="group-item__number">-->
    <!--                  <p>120</p>-->
    <!--                  <p>广播的数</p>-->
    <!--                </div>-->
    <!--                <div class="group-item__number">-->
    <!--                  <p>120</p>-->
    <!--                  <p>广播的数</p>-->
    <!--                </div>-->
    <!--                <div class="group-item__number">-->
    <!--                  <p>120</p>-->
    <!--                  <p>广播的数</p>-->
    <!--                </div>-->
    <!--              </div>-->
    <!--              <div class="group-item__avatars">-->
    <!--              <span class="group-item__avatar">-->
    <!--                  <img src="https://www.fillmurray.com/50/50" width="50" height="50"/>-->
    <!--              </span>-->
    <!--                <span class="group-item__avatar">-->
    <!--                  <img src="https://www.fillmurray.com/100/100" width="50" height="50"/>-->
    <!--              </span>-->
    <!--                <span class="group-item__avatar">-->
    <!--                <img src="https://www.fillmurray.com/200/200" width="50" height="50"/>-->
    <!--              </span>-->
    <!--                <span class="group-item__avatar">-->
    <!--                <img src="https://www.fillmurray.com/150/150" width="50" height="50"/>-->
    <!--              </span>-->
    <!--                <span class="group-item__avatar">-->
    <!--                  <img src="https://www.fillmurray.com/50/50" width="50" height="50"/>-->
    <!--              </span>-->
    <!--                <span class="group-item__avatar">-->
    <!--                  <p>+ 12</p>-->
    <!--              </span>-->
    <!--              </div>-->
    <!--              <div class="btn btn-blue-solid"><p>加入小组</p></div>-->
    <!--            </nuxt-link>-->
    <!--          </div>-->
    <!--          <div class="group-item">-->
    <!--            <nuxt-link to="/group-profile">-->
    <!--              <div class="group-item__top" style="background: url(data:image/jpeg;base64,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)"></div>-->
    <!--              <div class="group-item__button">-->
    <!--                <img draggable="false" src="/group_icon.png" alt="">-->
    <!--              </div>-->
    <!--              <div class="group-item__img">-->
    <!--                <img draggable="false" src="data:image/jpeg;base64,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" alt="">-->
    <!--              </div>-->
    <!--              <div class="group-item__title">我们爱坦克世界</div>-->
    <!--              <div class="group-item__subtitle">广播评级广播评级</div>-->
    <!--              <div class="group-item__numbers">-->
    <!--                <div class="group-item__number">-->
    <!--                  <p>120</p>-->
    <!--                  <p>广播的数</p>-->
    <!--                </div>-->
    <!--                <div class="group-item__number">-->
    <!--                  <p>120</p>-->
    <!--                  <p>广播的数</p>-->
    <!--                </div>-->
    <!--                <div class="group-item__number">-->
    <!--                  <p>120</p>-->
    <!--                  <p>广播的数</p>-->
    <!--                </div>-->
    <!--              </div>-->
    <!--              <div class="group-item__avatars">-->
    <!--              <span class="group-item__avatar">-->
    <!--                  <img src="https://www.fillmurray.com/50/50" width="50" height="50"/>-->
    <!--              </span>-->
    <!--                <span class="group-item__avatar">-->
    <!--                  <img src="https://www.fillmurray.com/100/100" width="50" height="50"/>-->
    <!--              </span>-->
    <!--                <span class="group-item__avatar">-->
    <!--                <img src="https://www.fillmurray.com/200/200" width="50" height="50"/>-->
    <!--              </span>-->
    <!--                <span class="group-item__avatar">-->
    <!--                <img src="https://www.fillmurray.com/150/150" width="50" height="50"/>-->
    <!--              </span>-->
    <!--                <span class="group-item__avatar">-->
    <!--                  <img src="https://www.fillmurray.com/50/50" width="50" height="50"/>-->
    <!--              </span>-->
    <!--                <span class="group-item__avatar">-->
    <!--                  <p>+ 12</p>-->
    <!--              </span>-->
    <!--              </div>-->
    <!--              <div class="btn btn-blue-solid"><p>加入小组</p></div>-->
    <!--            </nuxt-link>-->
    <!--          </div>-->


    <!--        </div>-->
    <!--      </div>-->
    <!--    </section>-->
    <div class="container">
      <p class="section-header style-simple text-center mb-60">有关我们<span>平台的问</span>题的答案</p>
      <div class="faq-wrapper mb-60">
        <vs-collapse>
          <vs-collapse-item>
            <div slot="header">
              如何使用我们的平台？
            </div>
            <p>
              在该网站上注册，填写您的个​​人资料，并放置头像。 然后，您可以充分利用我们的服务：与女孩见面并聊天，观看广播并参加小组讨论，提供礼物并从女孩那里购买商品！
            </p>
          </vs-collapse-item>

        </vs-collapse>
        <vs-collapse >
          <vs-collapse-item>
            <div slot="header">
              为什么要付费访问？
            </div>
            <p>
              与来自俄罗斯的女孩交流的经验是一个非常有趣的话题。 我们仅对真正感兴趣的交流对象提供对该网站的访问权限，因为否则，这些女孩将无法应付想要使用我们服务的大量人流！
            </p>
          </vs-collapse-item>

        </vs-collapse>
        <vs-collapse>
          <vs-collapse-item>
            <div slot="header">
              什么是水晶，我该如何使用它们？
            </div>
            <p>
              水晶是我们平台上的本地货币。 有了它，您可以方便快捷地向女孩赠送礼物并表现出关注的迹象，成为女孩的粉丝，为女孩自己订购女孩和商品的私人礼物，以及请求个人广播！<br><br>

              每月使用我们的平台，您将以常规价格获得300个晶体，以VIP速率获得1200个晶体。 如果您没有足够的货币，您总是可以立即从您的个人账户充值水晶的余额！
            </p>
          </vs-collapse-item>

        </vs-collapse>

      </div>

    </div>

    <div class="container">
      <p class="section-header style-simple text-center mb-60">我们女孩的评价</p>
      <div class="block-rounded p20">
        <vs-table :data="users">



          <template slot-scope="{data}">
            <vs-tr :key="indextr" v-for="(tr, indextr) in data" >
              <vs-td :data="data[indextr].id">
                {{data[indextr].id}}
              </vs-td>
              <vs-td :data="data[indextr].img">
                <img style="width: 40px;height: 40px;border-radius: 100%; object-fit: cover" :src="data[indextr].img" alt="">

              </vs-td>
              <vs-td :data="data[indextr].rating">
                {{data[indextr].rating}}
              </vs-td>

              <vs-td :data="data[indextr].name">
                {{data[indextr].name}}
              </vs-td>

              <vs-td :data="data[indextr].login">
                {{data[indextr].login}}
              </vs-td>


            </vs-tr>
          </template>
        </vs-table>
      </div>

    </div>


    <vs-popup class="holamundo" title="关于我们"  :active.sync="infoModal">
      <div class="banner-info-block">
        <div class="banner-info-block__top">

          <img class="banner-info-block__top--img" src="/lip.webp" alt="">

          <div class="banner-info-block__top--name">
            <p>Li pin hin</p>
            <p>creator QR SOCIAL</p>
          </div>
        </div>
        <div class="banner-info-block__content mb-20">
          <p class="section-subheader mb-10">我的传记</p>
          <p>我叫李品欣，1970年出生于湖北省十堰市。 1996年，我毕业于中国国家研究所俄罗斯和独联体文化与语言研究学院。 1998年，我第一次去俄罗斯出差，并于2001年返回，然后成为该国的常客！
在过去的六个月到两年的时间里，我一直进行了9次以上的商务旅行，并设法研究了这个国家和人民！
俄罗斯人对我们的文化和语言非常感兴趣，其中许多人希望交流和了解我们！唯一的障碍是俄罗斯的生活水平低下。</p>
        </div>
        <div class="banner-info-block__content">
          <p class="section-subheader mb-10">该门户网站背后的想法</p>
          <p class="mb-40">几年来，我一直在思考如何在我们这边的人与俄罗斯人之间建立桥梁和联系，并提出了一个这样的交流和相识的场所！
许多俄罗斯姑娘都梦想着移居中国并嫁给中国男人，所以我决定在这个网站上将双方的机会结合起来！
试试看，一定要写下您对我们门户网站的意见！ 我们会考虑您的每条评论，并不断完善和填充我们的网站！</p>
          <div class="btn btn-outline btn-outline-d-blue">
            <div class="btn-outline-inner">
              <p>
                写一条消息
              </p>
            </div>
          </div>
        </div>
      </div>

    </vs-popup>
  </div>
</template>

<script>
  import SocialGroup from '@/components/SocialGroup';
  // import Logo from '~/components/Logo.vue'
  // import VuesaxLogo from '~/components/VuesaxLogo.vue'

  export default {
    components: {
      //Logo,
      //VuesaxLogo
      SocialGroup
    },
    data(){
      return {

        showSideBlock:false,
        infoModal:false,
        users:[
          {
            "id": 1,
            "img":'https://media.gettyimages.com/photos/teenage-beauty-picture-id1126913832?s=2048x2048',
            "rating": "512 #1",
            "name": "LIZA MARKINA",
            "login": "@NATRY",
          },
          {
            "id": 2,
            "img":'https://images.unsplash.com/photo-1529626455594-4ff0802cfb7e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=634&q=80',
            "rating": "451 #2",
            "name": "LENKAA",
            "login": "@GODDESS",
          },
          {
            "id": 3,
            "img":'https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=634&q=80',
            "rating": "123 #3",
            "name": "KITTY PRETTY",
            "login": "@user12",
          },
          {
            "id": 4,
            "img":'https://images.unsplash.com/photo-1503185912284-5271ff81b9a8?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=634&q=80',
            "rating": "55 #4",
            "name": "LENKAA",
            "login": "@441",
          },
          {
            "id": 5,
            "img":'https://images.unsplash.com/photo-1496440737103-cd596325d314?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=634&q=80',
            "rating": "41 #5",
            "name": "LENKAA",
            "login": "@juiafuiui",
          },


        ]
      }
    },

  }
</script>

<style>
  .vs-collapse{
    background: #FDFDFD;
    border-radius: 8px;
  }
  .vs-collapse-item--header .vs-icon{
    font-size: 2rem;
  }
  .vs-collapse-item--header{
    font-weight: bold;
    font-size: 24px;
    line-height: 32px;
    /* identical to box height */


    letter-spacing: 0.05em;

    color: #545454;
  }

</style>
