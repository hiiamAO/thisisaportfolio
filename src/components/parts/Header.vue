<template>
  <header>
    <div class="header">
      <div class="logo menu-link">
        <router-link to="/">logo</router-link>
      </div>
      <div class="menu">
        <nav>
          <ul>
            <li class="menu-link">
              <router-link to="/projects">Projects</router-link>
            </li>

            <li class="menu-link">
              <router-link to="/about">About</router-link>
            </li>
          </ul>
        </nav>
      </div>
    </div>
  </header>
</template>

<style>
header {
  display: flex;

  position: fixed;
  width: 100%;
}

.header {
  display: inline-flex;
  justify-content: space-between;

  width: 100%;
  margin-left: 50px;
  margin-right: 50px;
  padding-top: 35px;

  font-size: 35px;
}

.router-link-active {
  color: #0038ff;
}

@media screen and (max-width: 600px) {
  .header {
    margin-left: 12.5px;
    margin-right: 12.5px;
    padding-top: 30px;
    font-size: 30px;
  }
}
</style>