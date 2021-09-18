<template>
  <div class="banner">
    <div class="wrapper">
      <button class="banner-btn">
        <a href="https://google.com/" target="_blank">My freelance profile</a>
      </button>
    </div>
  </div>
</template>

<style scoped>
.banner {
  display: flex;
  justify-content: center;

  width: 100%;
  height: 120px;
  background: #0038ff;
}

.wrapper {
  width: 700px;
}

.banner-btn {
  display: flex;
  justify-content: center;
  align-items: center;

  width: 100%;
  height: 70px;
  border-radius: 50px;

  font-size: 30px;
  text-transform: uppercase;
  color: #0038ff;
  background: #ffffff;
  transition: ease-out 0.3s;
}

.banner-btn a {
  display: inline-flex;
  justify-content: center;
  width: 100%;
  line-height: 48px;
  color: #0038ff;
}

.banner-btn a::after {
  display: block;
  content: "";
  width: 34px;
  height: 34px;
  margin-left: 15px;
  background-size: 34px;
  background-image: url("../../assets/images/man-computer-emoji.png");
  background-repeat: no-repeat;
}

.banner-btn:hover {
  transform: scale(1.1);
}
</style>