<template>
  <div class="center">
    <img src="/Logo.png" />
    <span class="title">em breve</span>
    <span class="subtitle">Vamos mudar a sua forma de ler</span>
    <span class="aguarde">AGUARDE!</span>
  </div>
  <div class="cover"></div>
  <div class="buttons">
    <a class="hide" href="https://www.google.com.br" target="_blank">
      <img class="brand" src="/Patreon.png" />
    </a>
    <a href="https://instagram.com/neomangas" target="_blank">
      <img class="brand" src="/Insta.png" />
    </a>

    <a href="https://discord.gg/GH7q57tfPj" target="_blank">
      <img class="brand" src="/Disc.png" />
    </a>
  </div>
</template>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Bebas+Neue&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Roboto+Condensed&display=swap");
@import "./assets/scss/responsividade.scss";

body {
  width: 100vw;
  height: 100vh;
  display: grid;
  align-items: center;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  background: linear-gradient(180deg, #000000 0%, rgba(0, 0, 0, 0) 100%);
  background-color: #222025;
  color: #fff;
  margin: 0;
  overflow: hidden;
  padding: 0%;
}
.hide {
  display: none;
}
.center {
  display: grid;
  grid-template-columns: 100%;
  grid-template-rows: 1fr;
  align-items: center;
  vertical-align: middle;
  img {
    margin: auto;
    height: 25vh;
    margin-bottom: max(3.75vw, 3.75vh);
  }
  .title {
    font-family: "Bebas Neue";
    text-align: center;
    font-size: max(16.5vw, 16.5vh);
    line-height: max(calc(14.5vw - 3.75vw), calc(16.5vh - 3.75vh));
  }
  .subtitle {
    font-family: "Roboto Condensed";
    text-align: center;
    font-size: max(3.75vw, 3.75vh);
    line-height: max(3.75vw, 3.75vh);
  }
}
.aguarde {
  font-family: "Bebas Neue";
  font-style: normal;
  font-weight: normal;
  margin-top: 4vh;
  font-size: max(5.75vw, 6.75vh);
  line-height: max(5.75vw, 6.75vh);
  text-align: center;
}
.cover {
  top: 0;
  left: 0;
  position: absolute;
  width: 100%;
  height: 100%;
  z-index: 99;
  display: block;
  background-color: transparent;
}

.buttons {
  z-index: 999;
  padding-top: 1rem;
  @include respond-above(md) {
    position: absolute;
    right: 2rem;
    bottom: 2rem;
  }
  .brand {
    width: 8vh;
    margin: 0.5rem;
    @include respond-below(md) {
      margin: auto;
      padding: 0.5rem;
    }
  }
}
</style>

