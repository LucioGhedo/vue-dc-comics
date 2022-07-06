<template>
  <div id="app">
    <header>
      <PageHeader />
    </header>
    <main>
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

export default {
  name: 'App',
  components: {
    PageHeader,
    ContentComponent,
    BlueBanner,
    FooterCompo,
    SignUp
}
}
</script>

<style lang="scss">
@import './style/common.scss';

</style>
