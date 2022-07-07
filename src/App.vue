<template>
  <div id="app">
    <header>
      <PageHeader />
    </header>
    <main>
      <UpBanner />
      <ContentComponent />
      <BlueBanner />
    </main>
    <footer>
      <FooterCompo />
      <SignUp />
    </footer>
  </div>
</template>

<script>
import PageHeader from './components/PageHeader.vue';
import ContentComponent from './components/ContentComponent.vue';
import BlueBanner from './components/BlueBanner.vue';
import FooterCompo from './components/FooterCompo.vue';
import SignUp from './components/SignUp.vue';
import UpBanner from './components/UpBanner.vue';

export default {
  name: 'App',
  components: {
    PageHeader,
    ContentComponent,
    BlueBanner,
    FooterCompo,
    SignUp,
    UpBanner
}
}
</script>

<style lang="scss">
@import './style/common.scss';
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap%27%27%27');

</style>
