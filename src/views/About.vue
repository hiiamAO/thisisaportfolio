<template>
  <div class="about">
    <Header />
    <PageTitle msg="About"/>
  </div>
</template>

<script>
// @ is an alias to /src
import PageTitle from '@/components/typography/PageTitle.vue'
import Header from '@/components/parts/Header.vue'

export default {
  name: 'Home',
  components: {
    Header,
    PageTitle
  }
}
</script>