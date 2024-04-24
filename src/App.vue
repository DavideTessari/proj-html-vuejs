<script>
import AppPageHeader from './components/AppPageHeader.vue';
import AppPageMain from './components/AppPageMain.vue';
import AppPageFooter from './components/AppPageFooter.vue';

export default {
  components: {
    AppPageHeader,
    AppPageMain,
    AppPageFooter
  },
  data() {
    return {
      links: [
        { text: 'Home' },
        { text: 'Services' },
        { text: 'Courses' },
        { text: 'About' },
        { text: 'FAQ' },
        { text: 'Blog' },
        { text: 'Contact Us' }
      ],
      address: '6767 Santa Monica Blvd, Los Angeles, CA 90038',
      phoneNumber: '123-456-789',
      copyright: 'Copyright © 2021, All Rights Reserved.',
      icons: [
        { text: '<i class="fa-brands fa-facebook-f"></i>' },
        { text: '<i class="fa-brands fa-telegram"></i>' },
        { text: '<i class="fa-brands fa-instagram"></i>' }
      ]
    };
  }
};
</script>

<template>
  <AppPageHeader :links="links" :address="address" :phoneNumber="phoneNumber"></AppPageHeader>

  <main>
    <AppPageMain></AppPageMain>
  </main>

  <AppPageFooter :copyright="copyright" :icons="icons"></AppPageFooter>
</template>

<style lang="scss">
@use './style/generic';
</style>