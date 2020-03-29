<template>
  <div>
    <nuxt/>
  </div>
</template>



<style>
/* Transitions using the page hook */
.page-enter-active, .page-leave-active {
  transition: all .5s ease-out;
}
.page-enter, .page-leave-active {
  opacity: 0;
  transform-origin: 50% 50%;
}
.clothrack {
font-family: 'Indie Flower', cursive;
  padding: 50px;
  width: 100vw;
  height: 100vh;
  display: flex;
  justify-content: space-evenly;
  flex-wrap: wrap;
}
.clothes {
  display: flex;
  justify-content: space-evenly;
  flex-wrap: wrap;
  width: 500px;
}
html, body {
font-family: 'Indie Flower', cursive;
  background: #9fdfbf;
  color: #000000;
  width: 100vw;
  height: 100vh;
}
h1 {
  width: 1000px;
  justify-content: center;
  display: flex;
}
a, a:visited {
  color: #ffffff;
  text-decoration: none;
}
</style>