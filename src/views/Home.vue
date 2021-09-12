<template>
  <div class="home">
    <Header />
    <PageTitle msg="This is a portfolio"/>
    <Banner />
    <Footer />
  </div>
</template>

<script>
import Header from '@/components/parts/Header.vue'
import PageTitle from '@/components/typography/PageTitle.vue'
import Banner from '@/components/parts/Banner.vue'
import Footer from '@/components/parts/Footer.vue'

export default {
  name: 'Home',
  components: {
    Header,
    PageTitle,
    Banner,
    Footer
  }
}
</script>
