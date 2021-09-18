<template>
  <div class="projects">
    <Header />
    <div class="scroll">
      <span>scroll</span>
    </div>
    <div class="project-list">
      <ul>
        <li v-for="project in projects" :key="project.project">
          <router-link :to="{ path: project.project }">{{
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
        { project: "riot" },
        { project: "supremesearcher" },
        { project: "mountain" },
        { project: "canicop" },
        { project: "Project #5" },
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
  color: #0038ff;
  font-size: 80px;
}

.project-list {
  display: flex;
  justify-content: center;

  width: 100%;
  padding-top: 150px;
  text-align: center;
}
ul {
  width: 100%;
  height: 100vh;
  /* padding-left: 75px;
  padding-right: 75px; */
}

ul li {
  font-size: 150px;
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

@media screen and (max-width: 1500px) {
  ul {
    width: 90%;
  }

  ul li {
    font-size: 100px;
    padding: 30px;
  }
}

@media screen and (max-width: 1200px) {
}

@media screen and (max-width: 900px) {
  ul li {
    font-size: 60px;
  }
}

@media screen and (max-width: 600px) {
  .project-list {
    padding-top: 60px;
  }
  .scroll {
    height: 33vh;
  }

  ul {
    width: 100%;
    height: 50vh;
  }

  ul li {
    font-size: 35px;
  }
}
</style>