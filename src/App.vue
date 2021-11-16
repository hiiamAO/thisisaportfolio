<template>
  <div id="app">
    <transition name="main-transition">
      <router-view />
    </transition>
  </div>
</template>

<style>
@import "./style.css";

.main-transition-enter-active {
  animation: transi 1.5s;
  animation-timing-function: ease-out;
}

@keyframes transi {
  from {
    transform: skew(0deg, 4deg);
    opacity: 0;
  }
  to {
    transform: skew(0deg, 0deg);
    opacity: 1;
  }
}
</style>
