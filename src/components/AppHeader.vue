<template>
  <header>
    <img alt="Vue logo" src="../assets/knf-logo-313x107.png" height="60">
    <p class="kongress">Kongress</p>
    <nav>
      <ul>
        <li><router-link to="/">Home</router-link></li>
        <li><router-link to="/program">Programm</router-link></li>
        <li><router-link to="/about">Über</router-link></li>
      </ul>
    </nav>
  </header>
</template>

<style lang="scss">
  header {
    display: flex;
    border-bottom: 1px solid #ccc;
    padding: .5rem 1rem;

    p {
      margin-left: 1rem;
    }

    .kongress {
	    color: #ff0000;
	    font-size: 110%;
    }
  }

  nav {
    margin-left: auto;

    ul {
      list-style: none;
    }

    ul li {
      display: inline-flex;
      margin-left: 1rem;
    }
  }
</style>
