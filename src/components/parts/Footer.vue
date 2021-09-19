<template>
  <footer>
    <div>
      <div class="footer-wrapper">
        <div>
          <ul class="footer-list">
            <li class="hoover-underline">Malt</li>
            <li class="hoover-underline">Linkedin</li>
            <li class="hoover-underline">Github</li>
            <li class="hoover-underline">arthuroberlin@gmail.com</li>
          </ul>
        </div>
        <!-- <a>
          <img class="footer-icon" src="@/assets/images/malt.png" />
        </a>
        <a>
          <img class="footer-icon" src="@/assets/images/github.svg" />
        </a> -->
      </div>
    </div>
    <div class="footer-wrapper">
      <div>
        <ul class="footer-list">
          <li>Arthur.O</li>
          <li>Front-end Developer</li>
          <li>Freelance</li>
          <li>Paris, France</li>
        </ul>
      </div>
    </div>
    <div class="footer-wrapper">
      <div>
        <ul class="footer-list">
          <li class="fact">"Give the best of yourself"</li>
          <br />
          <br />
          <li style="width: auto; text-align: right">© 2021</li>
        </ul>
      </div>
    </div>
  </footer>
</template>

<style scoped>
footer {
  display: flex;
  justify-content: space-evenly;
  flex-wrap: wrap;
  align-items: center;

  width: 100%;
  height: 300px;
  background: #0038ff;
  border-top: 1px solid white;
}

.footer-wrapper {
  display: flex !important;
  justify-content: center !important;
}

.footer-list li {
  width: fit-content;
  padding-bottom: 9px;

  font-family: "MonumentExtended-Regular";
  color: #ffffff;
  font-size: 22px;
}

.footer-icon {
  width: 25px;
  height: 25px;
}

.fact {
  font-family: "GloriaHallelujah"!important;
  font-size: 40px!important;
}
</style>