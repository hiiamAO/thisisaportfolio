<template>
  <div class="container">
    <div class="wrapper">
      <h1 class="title">{{ msg }}</h1>
    </div>
  </div>
</template>

<script>
export default {
  name: "PageTitle",
  props: {
    msg: String,
  },
};
</script>

<style>
.title {
  width: 100%;
  text-align: center;
  justify-content: center;
  font-family: "MonumentExtended-Ultrabold";
  font-size: 210px;
  text-transform: uppercase;
}

@media screen and (max-width: 1500px) {
  .title{
    font-size: 170px;
  }
}
@media screen and (max-width: 1200px) {
  .title{
    font-size: 120px;
  }
}
@media screen and (max-width: 900px) {
  .title{
    font-size: 80px;
  }
}
@media screen and (max-width: 600px) {
  .title{
    font-size: 50px;
  }
}
</style>
