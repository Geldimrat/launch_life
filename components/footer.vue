<template>
  <div class="footer_content">
    <div class="top_side">
      <div class="logo">
        <nuxt-link to="#home">
          <img src="~/static/logo.svg" alt="" />
        </nuxt-link>
      </div>
      <div class="social_medias">
        <nuxt-link to="" class="media_icon">
          <svg
            width="22"
            height="22"
            viewBox="0 0 22 22"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M20.9994 15.9738V18.9846C21.0005 19.2642 20.9432 19.5408 20.831 19.7969C20.7188 20.053 20.5542 20.2829 20.3478 20.4719C20.1415 20.6608 19.8978 20.8047 19.6325 20.8942C19.3672 20.9838 19.0861 21.017 18.8072 20.9919C15.7128 20.6563 12.7404 19.601 10.1289 17.9108C7.69921 16.3699 5.63926 14.3141 4.09534 11.8892C2.39586 9.27099 1.33824 6.29008 1.00816 3.18795C0.983033 2.91042 1.01608 2.63071 1.1052 2.36663C1.19432 2.10254 1.33757 1.85987 1.52581 1.65407C1.71405 1.44826 1.94317 1.28383 2.19858 1.17123C2.45398 1.05864 2.73008 1.00036 3.0093 1.0001H6.02608C6.5141 0.995304 6.98722 1.16778 7.35725 1.48537C7.72727 1.80297 7.96896 2.24401 8.03727 2.72629C8.1646 3.68982 8.40074 4.63587 8.74118 5.54642C8.87648 5.90563 8.90576 6.29602 8.82556 6.67133C8.74536 7.04665 8.55903 7.39115 8.28867 7.66402L7.01156 8.93859C8.44308 11.4512 10.5276 13.5315 13.0451 14.9602L14.3222 13.6856C14.5956 13.4158 14.9408 13.2298 15.3169 13.1498C15.6929 13.0698 16.0841 13.099 16.444 13.234C17.3564 13.5738 18.3043 13.8095 19.2698 13.9365C19.7582 14.0053 20.2044 14.2509 20.5233 14.6265C20.8422 15.0021 21.0116 15.4817 20.9994 15.9738Z"
              stroke="#09292B"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
          </svg>
        </nuxt-link>
        <nuxt-link to="" class="media_icon">
          <svg
            width="22"
            height="18"
            viewBox="0 0 22 18"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M3 1H19C20.1 1 21 1.9 21 3V15C21 16.1 20.1 17 19 17H3C1.9 17 1 16.1 1 15V3C1 1.9 1.9 1 3 1Z"
              stroke="#4285F4"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
            <path
              d="M21 3L11 10L1 3"
              stroke="#4285F4"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
          </svg>
        </nuxt-link>
        <nuxt-link to="" class="media_icon">
          <svg
            width="22"
            height="22"
            viewBox="0 0 22 22"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M16 1H6C3.23858 1 1 3.23858 1 6V16C1 18.7614 3.23858 21 6 21H16C18.7614 21 21 18.7614 21 16V6C21 3.23858 18.7614 1 16 1Z"
              stroke="#09292B"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
            <path
              d="M15.0002 10.3698C15.1236 11.2021 14.9815 12.052 14.594 12.7988C14.2065 13.5456 13.5933 14.1512 12.8418 14.5295C12.0903 14.9077 11.2386 15.0394 10.408 14.9057C9.57732 14.7721 8.80996 14.3799 8.21503 13.785C7.62011 13.1901 7.22793 12.4227 7.09426 11.592C6.9606 10.7614 7.09226 9.90971 7.47052 9.15819C7.84878 8.40667 8.45438 7.79355 9.20118 7.40605C9.94798 7.01856 10.7979 6.8764 11.6302 6.99981C12.4791 7.1257 13.265 7.52128 13.8719 8.12812C14.4787 8.73496 14.8743 9.52089 15.0002 10.3698Z"
              stroke="#09292B"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
            <path
              d="M16.5 5.5H16.51"
              stroke="#09292B"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
          </svg>
        </nuxt-link>
      </div>
    </div>
    <div class="bottom_side">
      <p class="secure">
        {{ new Date().getFullYear() }}, LaunchLife. All Rights Reserved.
      </p>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style></style>
