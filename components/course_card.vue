<template>
  <div class="course_card">
    <div class="course_logo">
      <img :src="require(`~/assets/images/courses/${card_info.img}`)" alt="" />
    </div>
    <p class="course_name">{{ card_info.name }}</p>
    <p class="description">
      {{ card_info.description }}
    </p>
    <div class="pro_langs">
      <div class="pro_logo" v-for="(e, i) in card_info.prog_langs" :key="i">
        <img :src="require(`~/assets/images/courses/${e}`)" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    card_info: {
      type: Object,
      required: true,
    },
  },
}
</script>

<style></style>
