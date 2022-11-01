<template>
  <header>
    <router-link to="/">
      <h1><span>Vue</span>Movies</h1>
    </router-link>
  </header>
  <main>
    <router-view />
  </main>
</template>

<style lang="scss">
  *{
    margin: 0;
    padding: 0;
    box-sizing: 0;
    font-family: 'Fira Sans';

    &::selection{
      background: transparentize($color: #B3ff00, $amount: 0.5);
    }
  }

  body{
    background-color: #000000;
  }

  a{
    text-decoration: none;
  }

  header{
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 10px 16px;
    background-color: #000000;
    box-shadow: 0px 0px 6px rgba(0, 0, 0, 0.1);
  }

  h1{
    color: #fff;
    font-size: 28px;
    text-shadow: 1px 1px 3px #b3ff00;
    
    span{
      color: #B3ff00;
    }
  }
</style>
