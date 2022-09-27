<template>
  <div class="nav_menu">
    <nuxt-link to="#home" class="logo">
      <img src="~/static/logo.svg" alt="" />
    </nuxt-link>
    <div class="links_r_side">
      <nav>
        <ul :class="toggle_nav_menu ? '' : 'top_nav_menu'">
          <li v-for="(e, i) in nav_menu" :key="i">
            <nuxt-link
              :to="e.href"
              @click.native="toggle_handler"
              class="links"
              >{{ e.name_en }}</nuxt-link
            >
          </li>
        </ul>
        <div
          v-if="toggle_nav_menu"
          class="back_opacity"
          @click="toggle_handler"
        ></div>
      </nav>
      <div class="lang_drop">
        <button class="dropbtn">
          <svg
            width="18"
            height="16"
            viewBox="0 0 18 16"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              fill-rule="evenodd"
              clip-rule="evenodd"
              d="M5.73063 0.807077V1.61415H2.86531H0V2.40406V3.19396H4.56956H9.13912L9.0327 3.4773C8.67146 4.43923 8.05002 5.56687 7.40151 6.43717C7.07012 6.88192 6.5885 7.45258 6.54458 7.45258C6.50879 7.45258 5.96692 6.81025 5.68988 6.43944C5.41175 6.06719 5.10599 5.59603 4.84857 5.143L4.65833 4.80818L3.8418 4.80815L3.02528 4.80812L3.149 5.07428C3.58132 6.00441 4.38214 7.21221 5.16973 8.12207L5.46009 8.45751L5.05951 8.83941C4.83918 9.04942 3.90147 9.95338 2.97574 10.8482L1.29255 12.4751L1.86773 13.0377L2.4429 13.6004L4.49105 11.5999L6.53917 9.59933L7.8139 10.8442L9.08863 12.0891L9.4004 11.2762L9.71222 10.4633L8.67599 9.45588L7.63977 8.44848L7.90341 8.148C9.0559 6.83443 10.0418 5.13912 10.5646 3.57174C10.6182 3.41119 10.6777 3.26052 10.6968 3.23689C10.7234 3.20409 11.0083 3.19396 11.905 3.19396H13.0785V2.40426V1.61457L10.222 1.60577L7.36544 1.59698L7.35601 0.798491L7.34656 0H6.53861H5.73063V0.807077ZM12.653 6.48175C12.6325 6.53402 11.8113 8.67092 10.8283 11.2304C9.84532 13.7898 9.03006 15.9113 9.01663 15.9447C8.99364 16.0019 9.04015 16.0049 9.81364 15.9962L10.6351 15.987L11.0921 14.7941L11.5491 13.6013H13.5004H15.4516L15.9086 14.7941L16.3657 15.987L17.1831 15.9962C17.6327 16.0013 18.0003 16.0013 18 15.9962C17.9998 15.9911 17.1716 13.8311 16.1597 11.196L14.3199 6.4051L13.5052 6.39589L12.6905 6.38665L12.653 6.48175ZM14.1624 10.2602C14.5139 11.181 14.8014 11.946 14.8013 11.9602C14.8013 11.9744 14.2158 11.9859 13.5004 11.9859C12.7849 11.9859 12.1995 11.9744 12.1994 11.9602C12.1991 11.9048 13.4787 8.58592 13.5004 8.58592C13.513 8.58592 13.811 9.33935 14.1624 10.2602Z"
              fill="#262626"
            />
          </svg>
        </button>
        <div class="lang-content">
          <div class="lang_content_inside">
            <button>English</button>
            <button class="active_lang">Русский</button>
            <button>Türkmen</button>
          </div>
        </div>
      </div>
      <div class="hamburger_menu" @click="toggle_handler">
        <svg
          v-if="!toggle_nav_menu"
          width="20"
          height="10"
          viewBox="0 0 20 10"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <rect y="0.25" width="20" height="2" fill="#4285F4" />
          <rect x="5" y="7.75" width="15" height="2" fill="#4285F4" />
        </svg>
        <svg
          v-else
          width="14"
          height="14"
          viewBox="0 0 14 14"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <rect
            width="16.8878"
            height="2"
            transform="matrix(0.713982 0.700164 -0.689114 0.724652 1.53491 0.332031)"
            fill="#4285F4"
          />
          <rect
            width="16.9668"
            height="2"
            transform="matrix(0.701652 -0.71252 0.701652 0.71252 0.534912 12.332)"
            fill="#4285F4"
          />
        </svg>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    const nav_menu = [
      {
        id: 1,
        name_tm: 'Biz barada',
        name_en: 'About us',
        name_ru: 'О нас',
        href: '#about_us',
      },
      {
        id: 2,
        name_tm: 'Kurslar',
        name_en: 'Courses',
        name_ru: 'Курсы',
        href: '#courses',
      },
      {
        id: 3,
        name_tm: 'Talyplar',
        name_en: 'Students',
        name_ru: 'Студенты',
        href: '#students',
      },
      {
        id: 4,
        name_tm: 'Habarlaşmak',
        name_en: 'Contact us',
        name_ru: 'Сряжитесъ с нами',
        href: '#contact_us',
      },
    ]
    return {
      nav_menu,
      toggle_nav_menu: false,
      scrollPosition: null,
    }
  },

  methods: {
    toggle_handler() {
      this.toggle_nav_menu ^= true
    },
  },
}
</script>

<style>
.change_color {
  background-color: red;
}
</style>
