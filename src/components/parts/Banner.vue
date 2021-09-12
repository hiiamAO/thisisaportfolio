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
  height: 100px;
  background: #0038ff;
}

.wrapper {
  width: 30%;
}

.banner-btn {
  display: flex;
  justify-content: center;
  align-items: center;

  width: 100%;
  height: 60px;
  border-radius: 50px;

  font-size: 30px;
  text-transform: uppercase;
  color: #0038ff;
  background: #ffffff;
}
.banner-btn a {
  color: #0038ff;
}
</style>