<template>
  <div>
    <full-page :options="options" id="fullpage" ref="fullpage">
      <div class="section">
        <button @click="$refs.fullpage.api.moveSectionDown()">
            Next
        </button>
        Section 1
      </div>
      <div class="section">
        <button @click="$refs.fullpage.api.moveSectionUp()">
            Prev
        </button>
        Section 2
      </div>
    </full-page>
  </div>
</template>


<script>
import Vue from 'vue'
import VueFullPage from 'vue-fullpage.js'
import 'fullpage.js/dist/fullpage.css'


Vue.use(VueFullPage);

export default {
    data: function(){
        return {
            options: {
                navigation: true,
            },
        }
    },
}
</script>

<style scoped>
</style>