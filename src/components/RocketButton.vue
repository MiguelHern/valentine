<template>
  <div class="rocket-wrapper">
    <div class="rocket-container">
      <div v-if="!showSVG" class="rocket" :class="{ 'launch': isRocketLaunched }">
        <button @click="launchRocket" :class="{ 'launch-body': isRocketLaunched }"
          class="rocket-body bg-red-500 text-white font-semibold py-2 px-6 rounded-full hover:bg-red-600 transition duration-300 ease-in-out transform focus:outline-none focus:ring-2 focus:ring-red-500 focus:ring-opacity-50">
          No
        </button>
        <div :class="{ 'hidden': !isRocketLaunched }">
          <div class="rocket-fin rocket-fin-left"></div>
          <div class="rocket-fin rocket-fin-right"></div>
          <div class="rocket-exhaust"></div>
          <div class="rocket-window">
          </div>
        </div>
      </div>
      <div v-show="showSVG" class="min-w-20 px-6">
        <svg width="48px" height="48px" viewBox="0 0 80 80" fill="none" xmlns="http://www.w3.org/2000/svg">
                <g id="SVGRepo_bgCarrier" stroke-width="0"></g>
                <g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g>
                <g id="SVGRepo_iconCarrier">
                    <path
                        d="M55.8624 68.7922C55.8624 65.8071 56.1166 61.5245 56.1166 59.5125C56.1166 57.5005 58.7774 55.0808 58.7774 45.6433C58.7774 36.2058 55.4679 34.2727 53.0483 34.3516C50.6286 34.4305 50.3305 32.5457 47.718 32.0416C45.7104 31.6515 45.3203 32.6333 44.0316 32.6333C42.7428 32.6333 42.0722 30.7222 39.898 30.7222C37.7238 30.7222 35.9485 32.4142 35.9485 32.4142C35.9485 32.4142 35.2384 31.3709 31.5914 31.498C26.8749 31.6602 27.4359 37.3061 27.4359 40.392C27.4359 43.4779 27.357 36.6749 27.357 36.6749C27.357 36.6749 19.9622 34.1763 21.1238 45.0779C21.2597 46.3578 19.857 56.1066 32.078 60.81C32.078 60.81 33.3974 61.2132 31.8544 69.9056C31.8544 69.9056 32.5163 73.9997 42.8656 73.9997C53.9907 73.9953 55.8624 68.7922 55.8624 68.7922Z"
                        fill="url(#paint0_linear)"></path>
                    <path
                        d="M35.9487 32.4145C35.9487 32.4145 37.1979 31.2266 38.8812 30.8408C38.0483 31.1214 36.4484 33.0588 35.7689 34.1109C35.7689 34.1109 33.2485 31.4194 31.5872 31.4983C35.129 31.3405 35.9487 32.4145 35.9487 32.4145Z"
                        fill="url(#paint1_linear)"></path>
                    <path
                        d="M47.3982 31.989C46.8459 31.9496 46.9818 33.3479 44.343 33.4882C44.343 33.4882 42.7387 32.6334 44.0274 32.6334C45.2504 32.629 45.6668 31.7567 47.3982 31.989Z"
                        fill="url(#paint2_linear)"></path>
                    <path
                        d="M54.7665 65.4653C54.3413 58.2677 48.8971 63.4007 54.7051 55.664C58.0234 51.2411 57.1861 42.9608 56.8223 39.6952C56.4585 36.4295 53.675 35.7632 51.7375 35.2811C50.0587 34.8603 49.4231 32.6905 48.0686 32.125C50.3611 32.7255 50.7425 34.4307 53.0482 34.3518C55.4678 34.2729 58.7773 36.206 58.7773 45.6435C58.7773 55.081 56.1166 57.5006 56.1166 59.5126C56.1166 61.5246 55.8623 65.8072 55.8623 68.7923C55.8623 68.7923 55.218 70.5807 52.4389 72.0623C52.9474 70.3528 54.9155 68.0734 54.7665 65.4653Z"
                        fill="url(#paint3_radial)"></path>
                    <path
                        d="M32.078 60.8104C25.6957 58.3557 23.4514 53.4244 22.0137 48.4404C24.898 56.2648 32.5032 58.816 33.5903 60.4466C34.5941 61.9545 35.3437 66.5483 32.6961 71.2912C31.9553 70.5285 31.8545 69.9017 31.8545 69.9017C33.3974 61.2093 32.078 60.8104 32.078 60.8104Z"
                        fill="url(#paint4_radial)"></path>
                    <path
                        d="M43.5581 73.9913C42.6946 68.626 46.6309 63.642 46.6309 55.4363C46.6309 46.424 52.5047 41.6942 49.261 32.603C50.5935 33.3438 51.2116 34.4134 53.0482 34.352C55.4679 34.2731 58.7774 36.2062 58.7774 45.6437C58.7774 55.0812 56.1166 57.5009 56.1166 59.5128C56.1166 61.5248 55.8624 65.8074 55.8624 68.7925C55.8624 68.7925 54.0652 73.7765 43.5581 73.9913Z"
                        fill="url(#paint5_radial)"></path>
                    <path
                        d="M34.252 35.3997C36.7944 35.3997 38.2453 34.5537 40.3011 34.5537C42.3569 34.5537 49.011 35.7986 49.011 40.239C49.011 44.6794 45.3815 53.6917 41.3882 54.8314C37.3949 55.9667 30.2981 50.5137 29.6932 46.8799C29.0883 43.246 30.2587 35.3997 34.252 35.3997Z"
                        fill="url(#paint6_radial)"></path>
                    <path
                        d="M44.3428 34.0101C44.3428 34.0101 44.3735 20.1541 44.3735 15.8013C44.3735 11.4442 44.7373 6 40.0164 6C35.2954 6 35.8609 11.808 35.8609 14.894C35.8609 17.9799 35.782 36.6752 35.782 36.6752"
                        fill="url(#paint7_linear)"></path>
                    <path
                        d="M44.3428 33.484C43.7203 33.5323 42.9971 32.98 42.9971 29.9948C42.9971 27.0097 42.756 15.4901 42.756 10.8393C42.756 8.05582 41.6777 6 40.0164 6C44.7329 6 44.3735 11.4442 44.3735 15.8013C44.3735 20.1584 44.3472 32.6117 44.3472 32.6117V33.484H44.3428Z"
                        fill="url(#paint8_linear)"></path>
                    <path
                        d="M40.0163 34.1989C36.5315 34.1989 38.2498 21.1451 38.2498 19.1199C38.2498 17.0948 36.7331 9.60791 39.5648 9.60791C40.9807 9.60791 42.1949 12.9481 41.2831 19.5232C40.3757 26.1027 43.5011 34.1989 40.0163 34.1989Z"
                        fill="url(#paint9_radial)"></path>
                    <path
                        d="M23.7493 36.8152C25.3931 39.8047 26.787 43.5613 27.5015 47.8308V42.3909L27.2867 36.6487C26.9316 36.5435 25.2747 36.1226 23.7493 36.8152Z"
                        fill="url(#paint10_radial)"></path>
                    <path
                        d="M27.471 36.7193L27.3614 36.6755C27.3614 36.6755 26.5812 36.4125 25.5686 36.43C25.7308 37.1095 25.836 37.8152 25.8711 38.5472C26.0639 42.6939 27.6463 48.0461 27.6463 48.0461L27.471 36.7193Z"
                        fill="url(#paint11_radial)"></path>
                    <path
                        d="M27.6814 48.3437C27.6814 48.3437 27.471 36.7977 27.471 36.7188C27.471 36.7188 27.3132 36.5566 26.8924 36.5566C26.7565 36.5566 26.6293 45.0298 27.6814 48.3437Z"
                        fill="#975500"></path>
                    <defs>
                        <linearGradient id="paint0_linear" x1="51.8136" y1="68.5334" x2="33.3908" y2="32.089"
                            gradientUnits="userSpaceOnUse">
                            <stop offset="0.00132565" stop-color="#FFCB4B"></stop>
                            <stop offset="1" stop-color="#FFD748"></stop>
                        </linearGradient>
                        <linearGradient id="paint1_linear" x1="42.018" y1="30.6739" x2="26.9398" y2="34.5313"
                            gradientUnits="userSpaceOnUse">
                            <stop stop-color="#FFBC47" stop-opacity="0"></stop>
                            <stop offset="1" stop-color="#E68E43"></stop>
                        </linearGradient>
                        <linearGradient id="paint2_linear" x1="50.9527" y1="31.3841" x2="40.0245" y2="34.1162"
                            gradientUnits="userSpaceOnUse">
                            <stop stop-color="#FFBC47" stop-opacity="0"></stop>
                            <stop offset="1" stop-color="#E68E43"></stop>
                        </linearGradient>
                        <radialGradient id="paint3_radial" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse"
                            gradientTransform="translate(49.3832 48.0607) rotate(180) scale(28.9435)">
                            <stop stop-color="#FFBC47" stop-opacity="0"></stop>
                            <stop offset="1" stop-color="#FF8900"></stop>
                        </radialGradient>
                        <radialGradient id="paint4_radial" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse"
                            gradientTransform="translate(29.7592 46.5552) rotate(180) scale(30.0741)">
                            <stop stop-color="#FFBC47" stop-opacity="0"></stop>
                            <stop offset="1" stop-color="#FF8900"></stop>
                        </radialGradient>
                        <radialGradient id="paint5_radial" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse"
                            gradientTransform="translate(45.7416 46.361) rotate(180) scale(25.0939 103.181)">
                            <stop stop-color="#FFBC47" stop-opacity="0"></stop>
                            <stop offset="1" stop-color="#FF8900"></stop>
                        </radialGradient>
                        <radialGradient id="paint6_radial" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse"
                            gradientTransform="translate(39.3416 39.4088) rotate(180) scale(10.3566 5.25668)">
                            <stop stop-color="#FBE07A"></stop>
                            <stop offset="0.2654" stop-color="#FCDF73" stop-opacity="0.7346"></stop>
                            <stop offset="0.6548" stop-color="#FDDB5F" stop-opacity="0.3452"></stop>
                            <stop offset="1" stop-color="#FFD748" stop-opacity="0"></stop>
                        </radialGradient>
                        <linearGradient id="paint7_linear" x1="54.7889" y1="76.0956" x2="41.6346" y2="29.2459"
                            gradientUnits="userSpaceOnUse">
                            <stop offset="0.00132565" stop-color="#FFCB4B"></stop>
                            <stop offset="1" stop-color="#FFD748"></stop>
                        </linearGradient>
                        <linearGradient id="paint8_linear" x1="47.6973" y1="18.3635" x2="36.7691" y2="21.0956"
                            gradientUnits="userSpaceOnUse">
                            <stop stop-color="#FFBC47" stop-opacity="0"></stop>
                            <stop offset="1" stop-color="#E68E43"></stop>
                        </linearGradient>
                        <radialGradient id="paint9_radial" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse"
                            gradientTransform="translate(39.7674 21.9024) rotate(91.5882) scale(12.7006 1.48173)">
                            <stop stop-color="#FBE07A"></stop>
                            <stop offset="0.2654" stop-color="#FCDF73" stop-opacity="0.7346"></stop>
                            <stop offset="0.6548" stop-color="#FDDB5F" stop-opacity="0.3452"></stop>
                            <stop offset="1" stop-color="#FFD748" stop-opacity="0"></stop>
                        </radialGradient>
                        <radialGradient id="paint10_radial" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse"
                            gradientTransform="translate(27.2065 31.241) scale(29.355)">
                            <stop stop-color="#FFBC47" stop-opacity="0"></stop>
                            <stop offset="1" stop-color="#FF8900"></stop>
                        </radialGradient>
                        <radialGradient id="paint11_radial" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse"
                            gradientTransform="translate(26.1122 30.6449) rotate(92.9961) scale(17.4604 3.67741)">
                            <stop stop-color="#FFBC47" stop-opacity="0"></stop>
                            <stop offset="1" stop-color="#FF8900"></stop>
                        </radialGradient>
                    </defs>
                </g>
            </svg>
      </div>

    </div>
  </div>
  <div :class="isRocketLaunched ? 'insulto' : 'hidden'"
    class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2">
    <svg width="48px" height="48px" viewBox="0 0 80 80" fill="none" xmlns="http://www.w3.org/2000/svg">
      <g id="SVGRepo_bgCarrier" stroke-width="0"></g>
      <g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g>
      <g id="SVGRepo_iconCarrier">
        <path
          d="M55.8624 68.7922C55.8624 65.8071 56.1166 61.5245 56.1166 59.5125C56.1166 57.5005 58.7774 55.0808 58.7774 45.6433C58.7774 36.2058 55.4679 34.2727 53.0483 34.3516C50.6286 34.4305 50.3305 32.5457 47.718 32.0416C45.7104 31.6515 45.3203 32.6333 44.0316 32.6333C42.7428 32.6333 42.0722 30.7222 39.898 30.7222C37.7238 30.7222 35.9485 32.4142 35.9485 32.4142C35.9485 32.4142 35.2384 31.3709 31.5914 31.498C26.8749 31.6602 27.4359 37.3061 27.4359 40.392C27.4359 43.4779 27.357 36.6749 27.357 36.6749C27.357 36.6749 19.9622 34.1763 21.1238 45.0779C21.2597 46.3578 19.857 56.1066 32.078 60.81C32.078 60.81 33.3974 61.2132 31.8544 69.9056C31.8544 69.9056 32.5163 73.9997 42.8656 73.9997C53.9907 73.9953 55.8624 68.7922 55.8624 68.7922Z"
          fill="url(#paint0_linear)"></path>
        <path
          d="M35.9487 32.4145C35.9487 32.4145 37.1979 31.2266 38.8812 30.8408C38.0483 31.1214 36.4484 33.0588 35.7689 34.1109C35.7689 34.1109 33.2485 31.4194 31.5872 31.4983C35.129 31.3405 35.9487 32.4145 35.9487 32.4145Z"
          fill="url(#paint1_linear)"></path>
        <path
          d="M47.3982 31.989C46.8459 31.9496 46.9818 33.3479 44.343 33.4882C44.343 33.4882 42.7387 32.6334 44.0274 32.6334C45.2504 32.629 45.6668 31.7567 47.3982 31.989Z"
          fill="url(#paint2_linear)"></path>
        <path
          d="M54.7665 65.4653C54.3413 58.2677 48.8971 63.4007 54.7051 55.664C58.0234 51.2411 57.1861 42.9608 56.8223 39.6952C56.4585 36.4295 53.675 35.7632 51.7375 35.2811C50.0587 34.8603 49.4231 32.6905 48.0686 32.125C50.3611 32.7255 50.7425 34.4307 53.0482 34.3518C55.4678 34.2729 58.7773 36.206 58.7773 45.6435C58.7773 55.081 56.1166 57.5006 56.1166 59.5126C56.1166 61.5246 55.8623 65.8072 55.8623 68.7923C55.8623 68.7923 55.218 70.5807 52.4389 72.0623C52.9474 70.3528 54.9155 68.0734 54.7665 65.4653Z"
          fill="url(#paint3_radial)"></path>
        <path
          d="M32.078 60.8104C25.6957 58.3557 23.4514 53.4244 22.0137 48.4404C24.898 56.2648 32.5032 58.816 33.5903 60.4466C34.5941 61.9545 35.3437 66.5483 32.6961 71.2912C31.9553 70.5285 31.8545 69.9017 31.8545 69.9017C33.3974 61.2093 32.078 60.8104 32.078 60.8104Z"
          fill="url(#paint4_radial)"></path>
        <path
          d="M43.5581 73.9913C42.6946 68.626 46.6309 63.642 46.6309 55.4363C46.6309 46.424 52.5047 41.6942 49.261 32.603C50.5935 33.3438 51.2116 34.4134 53.0482 34.352C55.4679 34.2731 58.7774 36.2062 58.7774 45.6437C58.7774 55.0812 56.1166 57.5009 56.1166 59.5128C56.1166 61.5248 55.8624 65.8074 55.8624 68.7925C55.8624 68.7925 54.0652 73.7765 43.5581 73.9913Z"
          fill="url(#paint5_radial)"></path>
        <path
          d="M34.252 35.3997C36.7944 35.3997 38.2453 34.5537 40.3011 34.5537C42.3569 34.5537 49.011 35.7986 49.011 40.239C49.011 44.6794 45.3815 53.6917 41.3882 54.8314C37.3949 55.9667 30.2981 50.5137 29.6932 46.8799C29.0883 43.246 30.2587 35.3997 34.252 35.3997Z"
          fill="url(#paint6_radial)"></path>
        <path
          d="M44.3428 34.0101C44.3428 34.0101 44.3735 20.1541 44.3735 15.8013C44.3735 11.4442 44.7373 6 40.0164 6C35.2954 6 35.8609 11.808 35.8609 14.894C35.8609 17.9799 35.782 36.6752 35.782 36.6752"
          fill="url(#paint7_linear)"></path>
        <path
          d="M44.3428 33.484C43.7203 33.5323 42.9971 32.98 42.9971 29.9948C42.9971 27.0097 42.756 15.4901 42.756 10.8393C42.756 8.05582 41.6777 6 40.0164 6C44.7329 6 44.3735 11.4442 44.3735 15.8013C44.3735 20.1584 44.3472 32.6117 44.3472 32.6117V33.484H44.3428Z"
          fill="url(#paint8_linear)"></path>
        <path
          d="M40.0163 34.1989C36.5315 34.1989 38.2498 21.1451 38.2498 19.1199C38.2498 17.0948 36.7331 9.60791 39.5648 9.60791C40.9807 9.60791 42.1949 12.9481 41.2831 19.5232C40.3757 26.1027 43.5011 34.1989 40.0163 34.1989Z"
          fill="url(#paint9_radial)"></path>
        <path
          d="M23.7493 36.8152C25.3931 39.8047 26.787 43.5613 27.5015 47.8308V42.3909L27.2867 36.6487C26.9316 36.5435 25.2747 36.1226 23.7493 36.8152Z"
          fill="url(#paint10_radial)"></path>
        <path
          d="M27.471 36.7193L27.3614 36.6755C27.3614 36.6755 26.5812 36.4125 25.5686 36.43C25.7308 37.1095 25.836 37.8152 25.8711 38.5472C26.0639 42.6939 27.6463 48.0461 27.6463 48.0461L27.471 36.7193Z"
          fill="url(#paint11_radial)"></path>
        <path
          d="M27.6814 48.3437C27.6814 48.3437 27.471 36.7977 27.471 36.7188C27.471 36.7188 27.3132 36.5566 26.8924 36.5566C26.7565 36.5566 26.6293 45.0298 27.6814 48.3437Z"
          fill="#975500"></path>
        <defs>
          <linearGradient id="paint0_linear" x1="51.8136" y1="68.5334" x2="33.3908" y2="32.089"
            gradientUnits="userSpaceOnUse">
            <stop offset="0.00132565" stop-color="#FFCB4B"></stop>
            <stop offset="1" stop-color="#FFD748"></stop>
          </linearGradient>
          <linearGradient id="paint1_linear" x1="42.018" y1="30.6739" x2="26.9398" y2="34.5313"
            gradientUnits="userSpaceOnUse">
            <stop stop-color="#FFBC47" stop-opacity="0"></stop>
            <stop offset="1" stop-color="#E68E43"></stop>
          </linearGradient>
          <linearGradient id="paint2_linear" x1="50.9527" y1="31.3841" x2="40.0245" y2="34.1162"
            gradientUnits="userSpaceOnUse">
            <stop stop-color="#FFBC47" stop-opacity="0"></stop>
            <stop offset="1" stop-color="#E68E43"></stop>
          </linearGradient>
          <radialGradient id="paint3_radial" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse"
            gradientTransform="translate(49.3832 48.0607) rotate(180) scale(28.9435)">
            <stop stop-color="#FFBC47" stop-opacity="0"></stop>
            <stop offset="1" stop-color="#FF8900"></stop>
          </radialGradient>
          <radialGradient id="paint4_radial" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse"
            gradientTransform="translate(29.7592 46.5552) rotate(180) scale(30.0741)">
            <stop stop-color="#FFBC47" stop-opacity="0"></stop>
            <stop offset="1" stop-color="#FF8900"></stop>
          </radialGradient>
          <radialGradient id="paint5_radial" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse"
            gradientTransform="translate(45.7416 46.361) rotate(180) scale(25.0939 103.181)">
            <stop stop-color="#FFBC47" stop-opacity="0"></stop>
            <stop offset="1" stop-color="#FF8900"></stop>
          </radialGradient>
          <radialGradient id="paint6_radial" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse"
            gradientTransform="translate(39.3416 39.4088) rotate(180) scale(10.3566 5.25668)">
            <stop stop-color="#FBE07A"></stop>
            <stop offset="0.2654" stop-color="#FCDF73" stop-opacity="0.7346"></stop>
            <stop offset="0.6548" stop-color="#FDDB5F" stop-opacity="0.3452"></stop>
            <stop offset="1" stop-color="#FFD748" stop-opacity="0"></stop>
          </radialGradient>
          <linearGradient id="paint7_linear" x1="54.7889" y1="76.0956" x2="41.6346" y2="29.2459"
            gradientUnits="userSpaceOnUse">
            <stop offset="0.00132565" stop-color="#FFCB4B"></stop>
            <stop offset="1" stop-color="#FFD748"></stop>
          </linearGradient>
          <linearGradient id="paint8_linear" x1="47.6973" y1="18.3635" x2="36.7691" y2="21.0956"
            gradientUnits="userSpaceOnUse">
            <stop stop-color="#FFBC47" stop-opacity="0"></stop>
            <stop offset="1" stop-color="#E68E43"></stop>
          </linearGradient>
          <radialGradient id="paint9_radial" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse"
            gradientTransform="translate(39.7674 21.9024) rotate(91.5882) scale(12.7006 1.48173)">
            <stop stop-color="#FBE07A"></stop>
            <stop offset="0.2654" stop-color="#FCDF73" stop-opacity="0.7346"></stop>
            <stop offset="0.6548" stop-color="#FDDB5F" stop-opacity="0.3452"></stop>
            <stop offset="1" stop-color="#FFD748" stop-opacity="0"></stop>
          </radialGradient>
          <radialGradient id="paint10_radial" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse"
            gradientTransform="translate(27.2065 31.241) scale(29.355)">
            <stop stop-color="#FFBC47" stop-opacity="0"></stop>
            <stop offset="1" stop-color="#FF8900"></stop>
          </radialGradient>
          <radialGradient id="paint11_radial" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse"
            gradientTransform="translate(26.1122 30.6449) rotate(92.9961) scale(17.4604 3.67741)">
            <stop stop-color="#FFBC47" stop-opacity="0"></stop>
            <stop offset="1" stop-color="#FF8900"></stop>
          </radialGradient>
        </defs>
      </g>
    </svg>
  </div>
</template>
<script setup>
import { ref } from 'vue';

const isRocketLaunched = ref(false);
const showSVG = ref(false);

const launchRocket = () => {
  isRocketLaunched.value = true;

  // Espera 1 segundo antes de mostrar el SVG
  setTimeout(() => {
    showSVG.value = true;
  }, 1500);
};
</script>

<style scoped>
.rocket-wrapper {
  display: inline-block;
  position: relative;
}

.rocket-body {
  /*border-radius: 50% 50% 0 0;*/
  position: relative;
  /*transform: scaleY(300%);*/
}

.rocket-window {
  width: 20px;
  height: 20px;
  background-color: #ecf0f1;
  border-radius: 50%;
  position: absolute;
  top: -70px;
  left: 50%;
  transform: translateX(-50%);
}

.rocket-fin {
  width: 0;
  height: 0;
  border-left: 10px solid transparent;
  border-right: 10px solid transparent;
  border-bottom: 20px solid #ff4500;
  /* Naranja más vibrante */
  position: absolute;
  bottom: -10px;
  filter: blur(2px);
  animation: flameFlicker 0.2s infinite alternate ease-in-out;
}

.rocket-fin-left {
  left: 10px;
  transform: rotate(-30deg);
}

.rocket-fin-right {
  right: 10px;
  transform: rotate(30deg);
}

.rocket-exhaust {
  width: 20px;
  height: 40px;
  background: radial-gradient(circle, rgba(255, 100, 0, 0.8), rgba(255, 0, 0, 0.4));
  clip-path: polygon(20% 0%, 80% 0%, 100% 100%, 0% 100%);
  position: absolute;
  bottom: -40px;
  left: 50%;
  transform: translateX(-50%);
  box-shadow: 0 0 20px rgba(255, 100, 0, 0.8);
  opacity: 0.9;
  filter: blur(3px);
  animation: flameGlow 0.3s infinite alternate ease-in-out;
}

@keyframes flameFlicker {
  0% {
    transform: scaleY(1) rotate(var(--rotation));
    opacity: 0.9;
    border-bottom-color: #ff4500;
    filter: blur(3px);
  }

  100% {
    transform: scaleY(1.3) rotate(var(--rotation));
    opacity: 0.6;
    border-bottom-color: #ffd700;
    filter: blur(5px);
  }
}

@keyframes flameGlow {
  0% {
    opacity: 0.8;
    transform: translateX(-50%) scaleY(1);
    box-shadow: 0 0 20px rgba(255, 100, 0, 0.8);
  }

  100% {
    opacity: 0.5;
    transform: translateX(-50%) scaleY(1.2);
    box-shadow: 0 0 40px rgba(255, 150, 0, 0.9);
  }
}

.rocket-fin-left {
  --rotation: -30deg;
}

.rocket-fin-right {
  --rotation: 30deg;
}

.launch-body {
  border-radius: 50% 50% 0 0;
  transform: scaleY(300%);
  transform-origin: bottom;
}

.launch {
  animation: launchAnimation 1.5s forwards 0.5s;
}

@keyframes launchAnimation {
  0% {}

  100% {
    transform: translate(-50%, -2000%);

  }
}

.insulto {
  animation: insultoAnimation 1s 1.5s 2;
}


@keyframes insultoAnimation {
  0% {
    transform: scale(100%);
    opacity: 1;
  }

  10% {
    transform: scale(500%);
    opacity: 1;
  }

  20% {
    transform: scale(100%);
    opacity: 1;
  }

  30% {
    transform: scale(500%);
    opacity: 1;
  }

  40% {
    transform: scale(100%);
    opacity: 1;
  }

  50% {
    transform: scale(500%);
    opacity: 1;
  }

  60% {
    transform: scale(100%);
    opacity: 1;
  }

  70% {
    transform: scale(500%);
    opacity: 1;
  }

  80% {
    transform: scale(100%);
    opacity: 1;
  }

  90% {
    transform: scale(500%);
    opacity: 1;
  }

  100% {
    transform: scale(100%);
    opacity: 0;
  }
}
</style>