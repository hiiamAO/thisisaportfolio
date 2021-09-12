<template>
  <ul>
    <li v-for="project in projects" :key="project.project">
      {{ project.project }}
    </li>
  </ul>
</template>


<script>
export default {
  data: function () {
    return {
      projects: [
        { project: "Project #1" },
        { project: "Project #2" },
        { project: "Project #3" },
        { project: "Project #4" },
        { project: "Project #5" },
      ],
    };
  },
};
</script>

<style scoped>
ul {
  width: 75%;
  height: 60vh;
  overflow: auto;
}

ul::-webkit-scrollbar {
  width: 8px;
  padding-left: 50px;
}
ul::-webkit-scrollbar-track {
  background: #ffffff; /* color of the tracking area */
}
ul::-webkit-scrollbar-thumb {
  background-color: #0038ff; /* color of the scroll thumb */
}

ul li {
  font-size: 140px;
  padding: 40px;
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