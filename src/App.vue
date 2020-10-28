<template>
  <nav class="navbar" role="navigation" aria-label="main navigation">
    <div class="navbar-brand is-text">
      DeckBuilder
    </div>

    <div class="navbar-menu">
      <div class="navbar-start">
        <router-link 
          to="/"
          class="navbar-item"
        >
          Home
        </router-link>
        <router-link 
          to="/about"
          class="navbar-item"
        >
          About
        </router-link>
      </div>
    </div>
  </nav>

  <router-view />

</template>

<style lang="scss">

  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
  }

  .navbar-brand.is-text {
    font-family: 'Times New Roman', Times, serif;
    line-height: 2;
    font-size: 1.5rem;
    margin: 0 .5em
  }

</style>
