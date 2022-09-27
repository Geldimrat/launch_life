<template>
  <div class="landing">
    <!-- home section starts -->
    <section class="home" id="home">
      <div class="home_sides">
        <div class="left">
          <div class="hooper">
            <hooper :settings="hooperSettings">
              <slide>
                <div class="img">
                  <img src="~/assets/images/home/slider1.png" alt="" />
                </div>
              </slide>
              <slide>
                <div class="img">
                  <img src="~/assets/images/home/slider1.png" alt="" />
                </div>
              </slide>

              <hooper-navigation slot="hooper-addons"></hooper-navigation>
            </hooper>
          </div>
        </div>
        <div class="right">
          <div class="content">
            <p class="title">
              <span>Learn a skill build</span> <br />
              Your portfolio <br />
              <b>Get hired!</b>
            </p>
            <p class="description">
              By pressing just one button, you will discover 1000 roads for
              yourself
            </p>
            <nuxt-link to="#courses" class="courses_btn">Courses</nuxt-link>
          </div>
        </div>
      </div>
      <div class="scroll_down">
        <nuxt-link to="" class="drop_content">
          <div class="icon">
            <svg
              width="16"
              height="7"
              viewBox="0 0 16 7"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M15 0.583374L8 6.41671L1 0.583374"
                stroke="#262626"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
          </div>
          <p class="text">Scroll down</p>
        </nuxt-link>
      </div>
    </section>
    <!-- home section ends -->

    <!-- partners section starts -->
    <section class="partners">
      <div class="top_side">
        <p class="title">Our partners</p>
        <div class="partners_slider">
          <hooper :settings="partnersSettings" class="hooper">
            <slide v-for="(e, i) in partners" :key="i">
              <div class="partner_logo">
                <img
                  :src="require(`~/assets/images/partners/${e.img}`)"
                  alt=""
                />
              </div>
            </slide>
          </hooper>
        </div>
      </div>
      <div class="bottom_side">
        <div class="shadow"></div>
      </div>
    </section>
    <!-- partners section end -->

    <!-- about section start -->
    <section class="about_us" id="about_us">
      <div class="about_content">
        <div class="information">
          <p class="title">About us</p>
          <p>
            Our site was created to help all women who are interested in
            technological areas such as Web Design, Programming and others.
          </p>
        </div>
        <div class="total_students">
          <TotalStudents />
        </div>
      </div>
    </section>
    <!-- about section end -->

    <!-- Advantages and goals section start -->
    <section class="adv_goals">
      <div class="left">
        <div class="goal_img">
          <div class="moon_vector">
            <svg
              width="102"
              height="101"
              viewBox="0 0 102 101"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <mask id="path-1-inside-1_85_4" fill="white">
                <path
                  d="M51 -3.17083e-06C61.0868 -4.05265e-06 70.9472 2.96177 79.3341 8.51078C87.721 14.0598 94.2578 21.9468 98.1179 31.1745C101.978 40.4022 102.988 50.556 101.02 60.3521C99.0522 70.1481 94.1949 79.1463 87.0624 86.2089C79.93 93.2714 70.8426 98.0811 60.9496 100.03C51.0566 101.978 40.8022 100.978 31.4831 97.1559C22.1641 93.3337 14.199 86.861 8.59505 78.5563C2.9911 70.2516 4.08772e-06 60.488 3.21454e-06 50.5L29.2357 50.5C29.2357 54.7624 30.5121 58.929 32.9036 62.4731C35.2951 66.0171 38.6943 68.7793 42.6712 70.4105C46.6481 72.0416 51.0241 72.4684 55.246 71.6368C59.4679 70.8053 63.3459 68.7528 66.3897 65.7388C69.4335 62.7249 71.5063 58.8849 72.3461 54.7044C73.1859 50.5239 72.7549 46.1907 71.1076 42.2528C69.4603 38.3149 66.6707 34.9491 63.0916 32.5811C59.5125 30.213 55.3046 28.9491 51 28.9491L51 -3.17083e-06Z"
                />
              </mask>
              <path
                d="M51 -3.17083e-06C61.0868 -4.05265e-06 70.9472 2.96177 79.3341 8.51078C87.721 14.0598 94.2578 21.9468 98.1179 31.1745C101.978 40.4022 102.988 50.556 101.02 60.3521C99.0522 70.1481 94.1949 79.1463 87.0624 86.2089C79.93 93.2714 70.8426 98.0811 60.9496 100.03C51.0566 101.978 40.8022 100.978 31.4831 97.1559C22.1641 93.3337 14.199 86.861 8.59505 78.5563C2.9911 70.2516 4.08772e-06 60.488 3.21454e-06 50.5L29.2357 50.5C29.2357 54.7624 30.5121 58.929 32.9036 62.4731C35.2951 66.0171 38.6943 68.7793 42.6712 70.4105C46.6481 72.0416 51.0241 72.4684 55.246 71.6368C59.4679 70.8053 63.3459 68.7528 66.3897 65.7388C69.4335 62.7249 71.5063 58.8849 72.3461 54.7044C73.1859 50.5239 72.7549 46.1907 71.1076 42.2528C69.4603 38.3149 66.6707 34.9491 63.0916 32.5811C59.5125 30.213 55.3046 28.9491 51 28.9491L51 -3.17083e-06Z"
                fill="white"
                stroke="#D6D6D6"
                stroke-width="2"
                mask="url(#path-1-inside-1_85_4)"
              />
            </svg>
          </div>
          <img src="~/assets/images/goal/1.png" alt="" />
          <div class="circle_vector">
            <svg
              width="101"
              height="102"
              viewBox="0 0 101 102"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <ellipse cx="50.5" cy="51" rx="50.5" ry="51" fill="#EBF9FA" />
            </svg>
          </div>
        </div>
      </div>
      <div class="right">
        <p class="title">Advantages and goals</p>
        <p class="description">
          Our site was created to help all women who are interested in
          technological areas such as Web Design, Programming and others. Our
          site was created to help all women who are interested in technological
          areas such as Web Design, Programming and others.
        </p>
        <div class="members_card">
          <div class="first_card">
            <svg
              width="52"
              height="69"
              viewBox="0 0 52 69"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M25.0125 0.248205C24.1088 0.731144 23.9786 1.20518 23.9786 4.01491C23.9786 6.85174 24.1064 7.30569 25.0409 7.78823C25.7067 8.13203 26.247 8.13203 26.9128 7.78823C27.8473 7.30569 27.9751 6.85174 27.9751 4.01491C27.9751 1.83791 27.9464 1.5204 27.7069 1.04528C27.2154 0.0701023 26.012 -0.285833 25.0125 0.248205ZM11.7756 3.79569C11.1254 4.09392 10.7238 4.77114 10.7238 5.56957C10.7238 6.17048 10.8451 6.46237 11.7892 8.13081C13.0693 10.3932 13.4324 10.8382 14.161 11.0367C15.5506 11.4154 16.9196 10.0658 16.589 8.64315C16.4522 8.0541 14.2008 4.25638 13.8162 3.96584C13.379 3.63538 12.318 3.54694 11.7756 3.79569ZM38.4186 3.8031C37.9257 4.02031 37.7792 4.22416 36.445 6.5492C35.0971 8.89823 35.012 9.4502 35.849 10.4149C36.64 11.3267 37.9462 11.3429 38.7203 10.4506C38.9287 10.2105 39.5785 9.16653 40.1645 8.13081C41.1086 6.46237 41.23 6.17048 41.23 5.56957C41.23 4.08987 39.803 3.1933 38.4186 3.8031ZM24.5115 12.1661C24.4016 12.1929 23.8621 12.2886 23.3126 12.3788C18.3141 13.1994 13.8707 17.0624 12.1524 22.0813C11.5661 23.7936 11.3899 24.9157 11.3899 26.935C11.3899 30.1618 12.1349 32.6457 13.8951 35.2873C14.7663 36.5946 16.3084 38.1576 17.6801 39.1236C18.9519 40.0192 19.7192 40.8493 20.1343 41.7789L20.4294 42.4397H22.204H23.9786V37.146V31.8521L22.2374 30.1014C19.9329 27.7845 19.645 27.1886 20.2504 25.9877C20.5521 25.3891 21.3195 24.9126 21.9818 24.9126C22.6504 24.9126 23.1682 25.2667 24.6114 26.7102L25.9769 28.0761L27.3423 26.7102C28.7856 25.2667 29.3034 24.9126 29.972 24.9126C30.6342 24.9126 31.4016 25.3891 31.7034 25.9877C32.3087 27.1886 32.0208 27.7845 29.7163 30.1014L27.9751 31.8521V37.146V42.4397H29.7498H31.5243L31.8194 41.7789C32.2345 40.8493 33.0018 40.0192 34.2736 39.1236C36.4473 37.5928 38.4824 35.0866 39.4378 32.7635C40.2575 30.771 40.5315 29.383 40.5486 27.1372C40.558 25.8904 40.4929 24.753 40.3788 24.1711C39.2231 18.2777 34.776 13.6936 28.9811 12.4227C28.1163 12.233 24.976 12.0527 24.5115 12.1661ZM2.00248 13.694C1.25728 14.1098 0.99911 14.5681 0.99911 15.4749C0.99911 16.0571 1.06985 16.3601 1.269 16.6298C1.56687 17.0338 5.30701 19.3136 5.90514 19.456C7.31082 19.7906 8.6443 18.4051 8.2701 16.9987C8.07321 16.2585 7.59284 15.8557 5.40572 14.5972C3.36314 13.4218 2.77153 13.2649 2.00248 13.694ZM48.1571 13.6992C47.1813 14.167 44.5654 15.7633 44.197 16.1158C43.2049 17.0648 43.5022 18.6591 44.7981 19.3372C45.5199 19.715 46.1225 19.5257 48.3378 18.2253C50.4892 16.9625 50.8707 16.6061 50.9835 15.754C51.198 14.1359 49.6275 12.994 48.1571 13.6992ZM20.6711 48.1544C20.7237 49.7557 20.7462 49.8658 21.2179 50.8318C21.8112 52.0468 22.5871 52.8139 23.8215 53.4056C24.6273 53.792 24.8315 53.8323 25.9838 53.8323C27.1847 53.8323 27.3127 53.804 28.2628 53.3288C29.4783 52.7208 30.2343 51.9378 30.8123 50.6882C31.1922 49.8666 31.2335 49.6428 31.2832 48.136L31.3376 46.4844H25.9769H20.6162L20.6711 48.1544ZM13.1216 48.6563C7.29737 49.5057 2.26691 53.9539 0.617983 59.7129C0.144138 61.3678 0 62.6414 0 65.1726C0 67.7692 0.145071 68.255 1.06225 68.7286C1.58352 68.9977 1.79653 69 25.9769 69C50.1572 69 50.3702 68.9977 50.8915 68.7286C51.8069 68.2559 51.9539 67.7668 51.9529 65.1966C51.9525 63.9496 51.867 62.429 51.7554 61.6787C50.6289 54.1159 44.1515 48.5107 36.5341 48.5073L35.3019 48.5068V48.9169C35.3019 49.8616 34.868 51.4612 34.2795 52.6863C33.765 53.7571 33.4761 54.1574 32.5181 55.127C31.56 56.0965 31.1645 56.389 30.1065 56.9097C28.7327 57.5857 27.301 57.9444 25.9769 57.9444C24.6527 57.9444 23.2211 57.5857 21.8472 56.9097C20.7892 56.389 20.3937 56.0965 19.4356 55.127C18.4845 54.1644 18.1839 53.7494 17.6676 52.6863C17.0736 51.4631 16.6518 49.8909 16.6518 48.8994V48.5068L15.2864 48.5232C14.5355 48.5323 13.5613 48.5921 13.1216 48.6563Z"
                fill="#4285F4"
              />
            </svg>
            <div class="content">
              <p class="name">Expert Teachers</p>
              <p class="info">
                Learn from industry experts who are passionate about teaching
              </p>
            </div>
          </div>
          <div class="first_card">
            <svg
              width="69"
              height="56"
              viewBox="0 0 69 56"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M22.5569 0.675832C18.9248 1.52586 16.3649 4.02067 15.4365 7.61485C15.1718 8.64009 15.1733 10.8956 15.4395 11.9401C16.2625 15.1699 18.6381 17.6742 21.8179 18.6638C22.6434 18.9207 23.1171 18.976 24.4381 18.9695C25.8349 18.9626 26.1944 18.9116 27.1256 18.5887C28.504 18.1105 29.306 17.6423 30.5327 16.5995L31.5213 15.7592L30.0408 14.2663L28.5604 12.7733L27.8672 13.3849C26.9722 14.1743 26.1776 14.5678 25.103 14.7535C21.7389 15.3345 18.7119 12.1691 19.4035 8.79308C19.7401 7.15006 20.7118 5.90178 22.221 5.17397C23.0088 4.79415 23.2195 4.75282 24.3709 4.75282C26.5513 4.75282 26.3465 4.59834 32.9708 11.2398C36.263 14.5406 39.0045 17.1771 39.444 17.4655C41.0292 18.5051 42.5313 18.955 44.4596 18.9676C46.1169 18.9784 46.9217 18.789 48.5579 18.0028C49.6474 17.4793 50.0024 17.2181 50.9812 16.2203C51.8846 15.2994 52.2486 14.805 52.6962 13.8908C55.2085 8.76042 52.6563 2.6587 47.2814 0.945083C44.023 -0.0937093 40.6582 0.706863 38.1122 3.12674L37.2568 3.93978L38.7357 5.42195L40.2148 6.90412L40.9594 6.19379C41.3691 5.80313 42.052 5.3191 42.4772 5.11814C43.1472 4.8016 43.4209 4.75282 44.5296 4.75282C45.7038 4.75282 45.8824 4.78927 46.7044 5.19741C48.7138 6.19488 49.8291 8.35078 49.4792 10.5609C49.0654 13.174 46.8097 14.9873 44.1834 14.8178C42.3171 14.6974 42.2936 14.6788 36.0613 8.42789C30.3028 2.65233 29.9142 2.2931 28.6708 1.59809C26.9966 0.66201 24.3325 0.260233 22.5569 0.675832ZM66.0907 9.83594C65.0541 10.0579 64.5802 10.7723 64.1498 12.761C63.7561 14.58 63.2339 18.6975 63.0774 21.2171C63.0009 22.447 62.8465 23.8091 62.7342 24.2441C62.2261 26.2108 57.8542 33.7162 55.2424 37.105C54.6986 37.8107 53.8992 37.7748 53.8992 37.0447C53.8992 36.854 55.2378 34.5117 57.092 31.458C60.499 25.847 60.6028 25.6197 60.2498 24.5412C59.7194 22.9207 57.6853 22.1982 56.4117 23.1779C56.1726 23.3617 54.511 25.4196 52.719 27.7508C49.1369 32.4109 48.5942 33.0323 47.0126 34.2848C45.5977 35.4055 43.6717 37.4501 42.8478 38.7064C42.046 39.9291 41.2813 41.6735 40.8816 43.1917C40.5098 44.6039 40.4985 45.8427 40.8102 51.0283C41.0401 54.8519 41.0457 54.8932 41.3811 55.1951L41.72 55.5H47.1345C52.6651 55.5 53.2685 55.4503 53.5212 54.9738C53.5875 54.8492 53.6852 53.4037 53.7385 51.7618L53.8354 48.7763L59.4677 41.9414C62.5655 38.182 65.2832 34.8186 65.5072 34.467C66.106 33.5269 66.6883 32.0441 66.8951 30.9335C66.9951 30.3965 67.4836 25.9426 67.9803 21.0361C68.9639 11.3237 68.9591 11.5298 68.2253 10.6505C67.6613 9.97442 66.8642 9.67035 66.0907 9.83594ZM1.12228 10.2655C0.728834 10.5682 0.435231 10.9432 0.262429 11.3636L0 12.002L0.91064 20.9796C1.41144 25.9172 1.90257 30.3943 2.00188 30.9287C2.21956 32.0996 2.7596 33.503 3.34802 34.4267C3.58612 34.8004 6.31925 38.1851 9.42177 41.9481L15.0627 48.7898L15.1595 51.7686C15.2127 53.4068 15.3152 54.8585 15.3875 54.9946C15.4596 55.1306 15.6702 55.3 15.8552 55.371C16.0486 55.4451 18.5509 55.5 21.736 55.5H27.2802L27.5631 55.1951C27.8238 54.9141 27.8643 54.5875 28.0815 51.0283C28.473 44.6089 28.4232 43.9329 27.3626 41.2726C26.3802 38.8087 24.5639 36.4513 22.221 34.5991C20.5717 33.2952 19.7682 32.3865 16.2988 27.9023C14.3867 25.4308 12.6443 23.2809 12.4269 23.1248C11.1576 22.2132 9.16539 22.96 8.64792 24.5412C8.29291 25.6261 8.39947 25.8609 11.7647 31.4061C13.4971 34.261 14.9482 36.6883 14.9893 36.8001C15.1397 37.2096 14.8634 37.6131 14.4326 37.6131C14.0835 37.6131 13.925 37.4745 13.3094 36.6307C11.2968 33.8721 8.63314 29.539 7.29103 26.8404C6.14927 24.5446 5.84277 23.469 5.83229 21.7212C5.82006 19.69 4.94718 13.208 4.48064 11.6848C4.10843 10.4697 3.53009 9.93797 2.49865 9.86277C1.77895 9.81032 1.67441 9.84095 1.12228 10.2655ZM6.7182 12.5171C6.96424 13.5709 7.54674 17.7713 7.64268 19.1843C7.68568 19.8177 7.75166 20.5918 7.78915 20.9044L7.85741 21.4728L8.4813 21.0738C8.82435 20.8544 9.18393 20.6748 9.28041 20.6748C9.51865 20.6748 9.50589 20.4812 9.1244 18.3001C8.6975 15.8587 8.16297 13.4388 7.96504 13.0519C7.73782 12.6073 7.28821 12.1383 6.88805 11.9283L6.53774 11.7444L6.7182 12.5171ZM62.0623 11.8895C61.6335 12.1287 61.1784 12.5829 60.9775 12.9722C60.6307 13.6445 59.3102 20.316 59.4884 20.4957C59.5177 20.5252 59.8792 20.7544 60.2918 21.0049L61.0422 21.4605L61.1097 20.8983C61.1468 20.5891 61.2123 19.8482 61.255 19.252C61.3577 17.8221 61.9521 13.4969 62.1816 12.5106C62.2813 12.0821 62.3558 11.7333 62.347 11.7355C62.3382 11.7378 62.2101 11.8071 62.0623 11.8895ZM10.0475 14.5432C10.3077 15.3947 11.0868 18.8501 11.17 19.5214L11.2703 20.3328L11.9015 20.4239C12.2487 20.4739 12.5952 20.554 12.6718 20.6017C12.8636 20.7212 12.748 20.1645 12.1096 17.8969C11.816 16.8535 11.4641 15.7788 11.3277 15.5088C10.9388 14.7383 9.85794 13.9231 10.0475 14.5432ZM58.0375 14.8819C57.5099 15.4215 57.4356 15.5988 56.8585 17.6937C55.9785 20.8884 56.0004 20.5758 56.6638 20.4718C57.6599 20.3159 57.6511 20.3241 57.7413 19.4545C57.8082 18.8085 58.5176 15.6729 58.8524 14.5432C58.973 14.1361 58.6252 14.2807 58.0375 14.8819Z"
                fill="#4285F4"
              />
            </svg>
            <div class="content">
              <p class="name">Unlimited Access</p>
              <p class="info">One subscription unlimited access</p>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- Advantages and goals section end -->

    <!-- Courses section start -->
    <section class="courses" id="courses">
      <div class="courses_content">
        <div class="top">
          <div class="title">
            <p class="name">Courses</p>
            <p class="info">
              Our site was created to help all women who are interested in
              technological areas such as Web Design, Programming and others.
            </p>
          </div>
          <div class="course_cards">
            <div :class="`card_${e.id}`" v-for="(e, i) in cards" :key="i">
              <CourseCard :card_info="e" />
            </div>
          </div>
        </div>
        <div class="bottom">
          <div class="vector_icon">
            <svg
              width="259"
              height="337"
              viewBox="0 0 259 337"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M333 168.5C333 201.826 323.235 234.404 304.94 262.114C286.644 289.823 260.641 311.42 230.217 324.174C199.793 336.927 166.315 340.264 134.017 333.762C101.72 327.261 72.0521 311.213 48.7667 287.647C25.4813 264.082 9.62368 234.058 3.19924 201.373C-3.2252 168.687 0.0720624 134.807 12.6741 104.018C25.276 73.2284 46.6168 46.9123 73.9976 28.3973C101.378 9.88229 133.569 -6.68737e-05 166.5 -6.83131e-05L166.5 51.8232C143.697 51.8232 121.407 58.6661 102.447 71.4868C83.4876 84.3074 68.7103 102.53 59.9842 123.85C51.258 145.17 48.9748 168.629 53.4234 191.262C57.872 213.896 68.8524 234.685 84.9763 251.003C101.1 267.32 121.643 278.433 144.008 282.935C166.372 287.437 189.553 285.126 210.62 276.295C231.687 267.464 249.693 252.51 262.362 233.322C275.03 214.135 281.792 191.576 281.792 168.5L333 168.5Z"
                fill="white"
                fill-opacity="0.2"
              />
            </svg>
          </div>
          <div class="choose_launchLife">
            <div class="question">
              <p class="title">Why Launch Life</p>
              <p class="description">
                Semaj Africa is an online education platform that delivers video
                courses, programs and resources for Individual, Advertising &
                Media Specialist
              </p>
            </div>
            <div class="advantages">
              <div class="card_plus" v-for="(e, i) in advantages" :key="i">
                <div class="vector_img">
                  <img
                    :src="require(`~/assets/images/courses/${e.img}`)"
                    alt=""
                  />
                </div>
                <p class="name">{{ e.name }}</p>
                <p class="text">
                  {{ e.text }}
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- Courses section end -->

    <!-- Students quote section start -->
    <section class="students" id="students">
      <div class="shadow"></div>
      <div class="vector_icon">
        <svg
          width="102"
          height="101"
          viewBox="0 0 102 101"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <mask id="path-1-inside-1_1_910" fill="white">
            <path
              d="M51 -3.17083e-06C61.0868 -4.05265e-06 70.9472 2.96177 79.3341 8.51078C87.721 14.0598 94.2578 21.9468 98.1179 31.1745C101.978 40.4022 102.988 50.556 101.02 60.3521C99.0522 70.1481 94.1949 79.1463 87.0624 86.2089C79.93 93.2714 70.8426 98.0811 60.9496 100.03C51.0566 101.978 40.8022 100.978 31.4831 97.1559C22.1641 93.3337 14.199 86.861 8.59505 78.5563C2.9911 70.2516 4.08772e-06 60.488 3.21454e-06 50.5L29.2357 50.5C29.2357 54.7624 30.5121 58.929 32.9036 62.4731C35.2951 66.0171 38.6943 68.7793 42.6712 70.4105C46.6481 72.0416 51.0241 72.4684 55.246 71.6368C59.4679 70.8053 63.3459 68.7528 66.3897 65.7388C69.4335 62.7249 71.5063 58.8849 72.3461 54.7044C73.1859 50.5239 72.7549 46.1907 71.1076 42.2528C69.4603 38.3149 66.6707 34.9491 63.0916 32.5811C59.5125 30.213 55.3046 28.9491 51 28.9491L51 -3.17083e-06Z"
            />
          </mask>
          <path
            d="M51 -3.17083e-06C61.0868 -4.05265e-06 70.9472 2.96177 79.3341 8.51078C87.721 14.0598 94.2578 21.9468 98.1179 31.1745C101.978 40.4022 102.988 50.556 101.02 60.3521C99.0522 70.1481 94.1949 79.1463 87.0624 86.2089C79.93 93.2714 70.8426 98.0811 60.9496 100.03C51.0566 101.978 40.8022 100.978 31.4831 97.1559C22.1641 93.3337 14.199 86.861 8.59505 78.5563C2.9911 70.2516 4.08772e-06 60.488 3.21454e-06 50.5L29.2357 50.5C29.2357 54.7624 30.5121 58.929 32.9036 62.4731C35.2951 66.0171 38.6943 68.7793 42.6712 70.4105C46.6481 72.0416 51.0241 72.4684 55.246 71.6368C59.4679 70.8053 63.3459 68.7528 66.3897 65.7388C69.4335 62.7249 71.5063 58.8849 72.3461 54.7044C73.1859 50.5239 72.7549 46.1907 71.1076 42.2528C69.4603 38.3149 66.6707 34.9491 63.0916 32.5811C59.5125 30.213 55.3046 28.9491 51 28.9491L51 -3.17083e-06Z"
            fill="white"
            stroke="#D6D6D6"
            stroke-width="2"
            mask="url(#path-1-inside-1_1_910)"
          />
        </svg>
      </div>
      <div class="circle_vector">
        <svg
          width="89"
          height="178"
          viewBox="0 0 89 178"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <ellipse cx="0.5" cy="89" rx="88.5" ry="89" fill="#EBF9FA" />
        </svg>
      </div>
      <div class="student_content">
        <div class="top">
          <p class="title">What Students Say</p>
          <p class="info">
            Semaj Africa is an online education platform that delivers video
            courses, programs and resources for Individual, Advertising & Media
            Specialist
          </p>
        </div>
        <div class="students_quote">
          <div class="quotes_slider">
            <hooper :settings="quotesSettings" class="hooper">
              <slide>
                <StudentCard />
              </slide>
              <slide>
                <StudentCard />
              </slide>
              <slide>
                <StudentCard />
              </slide>
              <hooper-navigation slot="hooper-addons"></hooper-navigation>
            </hooper>
          </div>
        </div>
      </div>
    </section>
    <!-- Students quote section end -->

    <!-- Contact section start -->
    <section class="contact_us" id="contact_us">
      <div class="left_side">
        <div class="forms">
          <p class="title">Contact us</p>
          <div class="input">
            <input type="text" placeholder="Name" />
          </div>
          <div class="input">
            <input type="email" placeholder="E-mail" />
          </div>
          <textarea placeholder="Comment" class="comment"></textarea>
          <div class="send_btn">
            <button class="send_data_btn">Send</button>
          </div>
        </div>
      </div>
      <div class="right_side">
        <div class="img_girl">
          <img src="~/assets/images/contact/Union.png" alt="" />
        </div>
      </div>
    </section>
    <!-- Contact section end -->
  </div>
</template>

<script>
import TotalStudents from '@/components/total_students.vue'
import CourseCard from '@/components/course_card.vue'
import StudentCard from '@/components/student_card.vue'
import { Hooper, Slide, Navigation as HooperNavigation } from 'hooper'
import 'hooper/dist/hooper.css'

export default {
  name: 'App',
  components: {
    Hooper,
    Slide,
    HooperNavigation,
    TotalStudents,
    CourseCard,
    StudentCard,
  },
  data() {
    const partners = [
      {
        img: '1.png',
        href: '',
      },
      {
        img: '2.png',
        href: '',
      },
      {
        img: '3.png',
        href: '',
      },
      {
        img: '4.png',
        href: '',
      },
    ]

    const cards = [
      {
        id: 1,
        img: 'web.png',
        name: 'Web development',
        description: 'Learn create web applications in HTML, CSS, JAVAScript',
        prog_langs: ['html.png', 'css.png', 'js.png'],
      },
      {
        id: 2,
        img: 'mobile.png',
        name: 'Mobile app development',
        description: 'Learn create mobile apps in Dart, Flutter',
        prog_langs: ['dart.png', 'flutter.png'],
      },
      {
        id: 3,
        img: 'design.png',
        name: 'UX and UI design',
        description:
          'Learn how to create modern design interfaces in Figma, Adobe XD',
        prog_langs: ['figma.png', 'xd.png'],
      },
    ]

    const advantages = [
      {
        id: 1,
        img: '1.svg',
        name: 'Save time',
        text: 'Learn more in short time with flexible schedule',
      },
      {
        id: 2,
        img: '2.svg',
        name: 'Comunity',
        text: 'Ask about lessons or random things on chatting groups',
      },
      {
        id: 3,
        img: '3.svg',
        name: 'Activities',
        text: 'Meetings, guests, speaking days and etc.',
      },
    ]

    return {
      partners,
      cards,
      advantages,
    }
  },
  computed: {
    hooperSettings() {
      const settings = {
        itemsToShow: 1,
        centerMode: false,
        autoPlay: true,
        playSpeed: 3000,
        transition: 1100,
        hoverPause: false,
        infiniteScroll: true,
        wheelControl: false,
      }
      return settings
    },

    partnersSettings() {
      const settings = {
        itemsToShow: 4,
        centerMode: false,
        // autoPlay: true,
        playSpeed: 3000,
        transition: 1100,
        hoverPause: false,
        infiniteScroll: true,
        wheelControl: false,
      }
      return settings
    },

    quotesSettings() {
      const settings = {
        itemsToShow: 3,
        centerMode: false,
        // autoPlay: true,
        playSpeed: 3000,
        transition: 1100,
        hoverPause: false,
        infiniteScroll: true,
        wheelControl: false,
      }
      return settings
    },
  },

  // mounted() {


  //   window.onscroll = () => {

  //   }
  // },
}
</script>

<style scoped></style>
