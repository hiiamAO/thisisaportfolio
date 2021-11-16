<template>
  <div class="projects">
    <Header />
    <div class="scroll">
      <span>scroll</span>
    </div>
    <div class="project-list">
      <ul>
        <li v-for="project in projects" :key="project.project">
          <router-link :to="{ path: project.link }">{{
            project.project
          }}</router-link>
        </li>
      </ul>
    </div>
    <Banner />
    <Footer />
  </div>
</template>

<script>
import Header from "@/components/parts/Header.vue";
import Banner from "@/components/parts/Banner.vue";
import Footer from "@/components/parts/Footer.vue";

export default {
  name: "Home",
  components: {
    Header,
    Banner,
    Footer,
  },
  data: function () {
    return {
      projects: [
        { project: "riot", link: "project/sumsearch" },
        { project: "s.searcher", link: "project/sumsearch" },
        { project: "mountain", link: "project/sumsearch" },
        { project: "canicop", link: "project/sumsearch" },
        { project: "Project #5", link: "project/sumsearch" },
      ],
    };
  },
};
</script>

<style scoped>
.scroll {
  display: flex;
  justify-content: center;
  align-items: end;

  width: 100%;
  height: 25vh;
}

.scroll span {
  font-family: "Pangolin" !important;
  font-family: "GloriaHallelujah" !important;
  color: #0038ff;
  font-size: 90px;
  line-height: 50px;
}

.project-list {
  display: flex;
  justify-content: center;

  width: 100%;
  padding-top: 180px;
  text-align: center;
}
ul {
  width: 100%;
  height: 100vh;
  /* padding-left: 75px;
  padding-right: 75px; */
}

ul li {
  font-size: 8vw;
  text-transform: uppercase;
  transition: ease-in background 0.1s;
}

ul li:hover {
  background: #0038ff;
}

ul li a {
  display: block;
  padding-top: 40px;
  padding-bottom: 40px;
  transition: ease-in color 0.1s;
}

ul li a:hover {
  color: #ffffff !important;
}

@media screen and (min-width: 1500px) {
  .project-list {
    height: 110vh;
  }
}

@media screen and (max-width: 1200px) {
}

@media screen and (max-width: 900px) {
}

@media screen and (max-width: 600px) {
}
</style>