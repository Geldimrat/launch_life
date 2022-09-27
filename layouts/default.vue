<template>
  <div class="main">
    <div class="header">
      <Header />
    </div>
    <nuxt />
    <div class="footer">
      <Footer />
    </div>
  </div>
</template>

<script>
import Header from '@/components/header.vue'
import Footer from '@/components/footer.vue'
export default {
  components: {
    Header,
    Footer,
  },
  mounted() {
    let nav_bar = document.querySelector('.header')

    let section = document.querySelectorAll('section')
    let links = document.querySelectorAll('.links')

    function activeLink(a) {
      links.forEach((item) => item.classList.remove('active_link'))
      a.classList.add('active_link')
    }

    window.onscroll = () => {
      if (scrollY > 80) {
        nav_bar.classList.add('scrolled_nav')
      } else {
        nav_bar.classList.remove('scrolled_nav')
      }

      section.forEach((sec) => {
        let top = window.scrollY
        let offset = sec.offsetTop
        let height = sec.offsetHeight

        if (top >= offset && top < offset + height) {
          // let listsArray = Array.from(links)
          let sec_id = sec.getAttribute('id')
          // let target = ''
          links.forEach((e) => {
            if (e.getAttribute('href').includes(sec_id)) {
              activeLink(e)
              console.log(e);
            }
          })
          // activeLink(target)
          // console.log(target)
          // console.log(link_href)
        }
      })
    }
  },
}
</script>

<style></style>
