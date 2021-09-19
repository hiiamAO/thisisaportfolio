<template>
  <div>
    <header style="z-index: 1">
      <div class="header">
        <div class="logo menu-link">
          <router-link to="/projects">back</router-link>
        </div>
        <div class="menu">
          <nav>
            <ul>
              <li class="menu-link">
                <a class="link-0" href="#sld-0">Information</a>
              </li>
              <li class="menu-link">
                <a class="link-1" href="#sld-1">In picture</a>
              </li>
              <li class="menu-link">
                <a class="link-2" href="#sld-2">2</a>
              </li>
            </ul>
          </nav>
        </div>
      </div>
    </header>

    <full-page :options="options" id="fullpage" ref="fullpage">
      <div class="section" data-anchor="sld-0">
        <PageTitle msg="Sum Search" />
      </div>
      <div class="section" data-anchor="sld-1">
        <Project-infos />
      </div>
      <div class="section" data-anchor="sld-2">
        <Banner />
        <Footer />
      </div>
    </full-page>
  </div>
</template>

<script>
import Vue from "vue";
import VueFullPage from "vue-fullpage.js";
import "fullpage.js/dist/fullpage.css";

Vue.use(VueFullPage);

import PageTitle from "@/components/typography/PageTitle.vue";
import ProjectInfos from "@/components/project/Project-infos.vue";
import Banner from "@/components/parts/Banner.vue";
import Footer from "@/components/parts/Footer.vue";

export default {
  data: function () {
    return {
      options: {
        anchors: ["sld-0", "sld-1", "sld-2"],
        navigation: true,
      },
    };
  },
  components: {
    PageTitle,
    ProjectInfos,
    Banner,
    Footer,
  },
};
</script>

<style>
div#fp-nav {
  right: 28.5vh !important;
  top: 5vh;
}

#fp-nav ul li a {
  margin-top: 35px !important;
}

#fp-nav ul li a span {
  height: 8px;
  width: 8px;
  background: #0038ff !important;
  margin: -4px 0 0 -4px;
}
</style>

<style scoped>
.menu-link button {
  cursor: pointer;
  transition: all 0.2s;
}
.menu-link button:hover {
  color: #0038ff !important;
}

.fp-viewing-sld-0 .link-0 {
  color: #0038ff !important;
}
.fp-viewing-sld-1 .link-1 {
  color: #0038ff !important;
}
.fp-viewing-sld-2 .link-2 {
  color: #0038ff !important;
}
</style>