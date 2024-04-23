<script>
import AppPageHeader from './components/AppPageHeader.vue';
import AppPageMain from './components/AppPageMain.vue'
import AppPageFooter from './components/AppPageFooter.vue'

export default {
  components: {
    AppPageHeader,
    AppPageMain,
    AppPageFooter
  },
  data() {
    return {
      links: [
        {
          text: 'Home',
          active: true
        },
        {
          text: 'Services',
          active: true
        },
        {
          text: 'Courses',
          active: false
        },
        {
          text: 'About',
          active: false
        },
        {
          text: 'FAQ',
          active: false
        },
        {
          text: 'Blog',
          active: true
        },
        {
          text: 'Contact Us',
          active: false
        },
      ],
    };
  }
}
</script>

<template>
  <AppPageHeader :links="links"></AppPageHeader>

  <main>
    <AppPageMain></AppPageMain>
  </main>

  <AppPageFooter></AppPageFooter>
</template>

<style lang="scss">
@use './style/generic';
</style>