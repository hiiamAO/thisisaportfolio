<template>
  <div class="about">
    <Header />
    <PageTitle msg="About me" />
    <div class="container" style="padding-bottom: 150px">
      <div class="left">
        <div class="about-text">
          <span>Get in Touch</span>
        </div>
      </div>
      <div class="right">
        <div class="about-text">
          <p>
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Odit sit
            aut nihil, quasi earum culpa neque et doloribus corrupti ipsam
            repudiandae officia nemo molestiae quo ab rerum architecto impedit
            quae?
          </p>
        </div>
      </div>
    </div>
    <Banner />
    <Footer />
  </div>
</template>

<script>
import PageTitle from "@/components/typography/PageTitle.vue";
import Header from "@/components/parts/Header.vue";
import Banner from "@/components/parts/Banner.vue";
import Footer from "@/components/parts/Footer.vue";

export default {
  name: "Home",
  components: {
    Header,
    PageTitle,
    Banner,
    Footer,
  },
};
</script>

<style scoped>
.container {
  display: flex;
  flex-wrap: wrap;
  align-items: center;

  width: 100%;
  height: 80vh;
}
.left {
  width: 40%;
}
.right {
  width: 60%;
}

.about-text {
  padding: 100px;
}

.about-text span {
  font-family: "Pangolin";
  font-size: 130px;
  color: #0038ff;
}

.about-text p {
  font-family: "MonumentExtended-Regular";
  font-size: 50px;
  line-height: 70px;
}

@media screen and (max-width: 1200px) {
  .about-text {
    padding: 50px;
  }
}

@media screen and (max-width: 1000px) {
  .left {
    width: 100%;
  }
  .right {
    width: 100%;
  }
  .about-text span {
    font-size: 100px;
  }

  .about-text p {
    font-size: 40px;
    line-height: 50px;
  }
}

@media screen and (max-width: 600px) {
  .about-text span {
    font-size: 80px;
  }

  .about-text p {
    font-size: 30px;
    line-height: 40px;
  }
}
</style>