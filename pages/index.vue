<template>
  <div class="home--page">
    <b-container class="home--page__container">
      <!-- <Logo /> -->
      <b-row>
        <b-col cols="12" class="text-center mb-5">
          <h3>illusion wiki</h3>
          <p class="home--text__title">illusion wiki</p>
          <span class="home--text">is coming...</span>
        </b-col>
      </b-row>
      <b-row no-gutters>
        <b-col cols="4" md="2" v-for="(link, key) in listsImage" :key="key">
          <div class="home--group">
            <img class="home--img" :src="link.src" alt="" />
          </div>
        </b-col>
      </b-row>
      <b-row>
        <b-col cols="12" class="mt-5">
          <a href="https://www.facebook.com/ZendohTV" target="_bank">
            <b-button class="home--btn facebook">FACEBOOK</b-button>
          </a>
        </b-col>
      </b-row>
      <!-- <h3 class="mt-3">{{ test }}</h3> -->
    </b-container>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  data() {
    return {
      test: '',
      listsImage: [
        {
          src:
            'https://cdn.discordapp.com/attachments/319672282694025227/815973137325228082/2.png',
        },
        {
          src:
            'https://cdn.discordapp.com/attachments/319672282694025227/815973263427108924/P.png',
        },
        {
          src:
            'https://cdn.discordapp.com/attachments/319672282694025227/815979424125681696/848e5c86702c09e9.png',
        },
        {
          src:
            'https://cdn.discordapp.com/attachments/319672282694025227/815980853866921994/2.png',
        },
        {
          src:
            'https://cdn.discordapp.com/attachments/319672282694025227/815993451250057236/5c675bfa7e5d158b.png',
        },
        {
          src:
            'https://cdn.discordapp.com/attachments/319672282694025227/816020176561635398/001.png',
        },
      ],
    }
  },
  mounted() {
    this.test = process.env.TEST || 'Hello !!'
  },
})
</script>
<style lang="scss" scoped>
@import './style.scss';
</style>
