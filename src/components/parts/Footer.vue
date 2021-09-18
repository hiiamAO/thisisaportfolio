<template>
  <footer>
    <div>
      <div class="footer-wrapper">
        <a>
          <img class="footer-icon" src="@/assets/images/malt.png" />
        </a>
        <a>
          <img class="footer-icon" src="@/assets/images/github.svg" />
        </a>

        <span>arthuroberlin@gmail.com</span>
      </div>
    </div>
    <div class="footer-wrapper">
      <div>2</div>
    </div>
    <div class="footer-wrapper">
      <div>3</div>
    </div>
  </footer>
</template>

<style scoped>
footer {
  display: flex;
  justify-content: space-evenly;
  flex-wrap: wrap;

  width: 100%;
  color: #ffffff !important;
  background: #000000;
}

footer div {
  display: flex;
  width: 25%;
}

.footer-wrapper {
  display: flex !important;
  justify-content: center !important;
  color: #ffffff !important;
}

.footer-wrapper span {
    color: #ffffff !important;
    font-family: "MonumentExtended-Regular";
    letter-spacing: 1px;
}

.footer-icon {
  width: 25px;
  height: 25px;
}
</style>