<template>
  <div class="projects">
    <Header />
    <div class="scroll">
      <span>scroll</span>
    </div>
    <div class="project-list">
      <Project-list />
    </div>
  </div>
</template>

<script>
import Header from "@/components/parts/Header.vue";
import ProjectList from "../components/project/Project-list.vue";

export default {
  name: "Home",
  components: {
    Header,
    ProjectList,
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
  font-size: 55px;
}

.project-list {
    display: flex;
    justify-content: center;

    width: 100%;
    padding-top: 150px;
    text-align: center;
}

@media screen and (max-width: 600px) {
  .project-list {
    padding-top: 60px;
  }
}
</style>