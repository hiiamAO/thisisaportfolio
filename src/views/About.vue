<template>
  <div class="about">
    <Header />
    <PageTitle msg="About me" />
    <div class="container about-intro" style="height: 80vh">
      <div class="left">
        <div class="about-text" style="text-align: center">
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
    <div class="container">
      <div class="sketch">
        <span>I live and work here</span>
        <img class="sketch-img" src="@/assets/images/paris.png" />
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
  align-items: center;
  width: 100%;
  height: 100vh;
}
.left {
  width: inherit;
}

.about-text {
  padding: 80px;
}

.about-text span {
  font-family: "GloriaHallelujah" !important;
  font-size: 130px;
  color: #0038ff;
  line-height: 150px;
}

.about-text p {
  font-family: "MonumentExtended-Regular";
  font-size: 50px;
  line-height: 70px;
}

.sketch {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
}

.sketch span {
  font-family: "GloriaHallelujah" !important;
  font-size: 80px;
  color: #0038ff;
  line-height: 100px;
  padding: 40px;
  text-align: center;

  width: 20%;
}

.sketch img {
  max-width: 1000px;
  object-fit: contain;
}

@media screen and (max-width: 1400px) {
  .sketch img {
    max-width: 800px;
  }
}

@media screen and (max-width: 1200px) {
  .about-text {
    padding: 50px;
  }
  .about-text p {
    font-size: 40px;
    line-height: 55px;
  }
  .sketch span {
    line-height: 80px;
    padding: 30px;
  }
  .sketch img {
    max-width: 650px;
  }
}

@media screen and (max-width: 1000px) {
  .about-intro {
    flex-wrap: wrap;
  }
  .left {
    width: 100%;
  }
  .right {
    width: 100%;
  }

  .about-text {
    padding: 50px;
  }

  .about-text span {
    font-size: 100px;
  }
  .about-text p {
    font-size: 35px;
    line-height: 50px;
    text-align: center;
    margin-top: -120px;
  }
  .sketch span {
    width: 100%;
    line-height: 100px;
    padding: 40px;
  }
  .sketch img {
    width: 100%;
    max-width: 800px;
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
  .sketch span {
    font-size: 60px;
    line-height: 80px;
    padding: 40px;
  }

  .sketch img {
    width: 100%;
    width: 350px;
  }
}
</style>