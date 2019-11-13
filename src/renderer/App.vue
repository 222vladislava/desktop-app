<template>
  <div id="app">
    <router-view></router-view>
  </div>
</template>

<script>
  export default {
    name: 'desktop-app'
  }
</script>

<style lang="scss">
  @import url('https://fonts.googleapis.com/css?family=Open+Sans:300,400,700|Roboto:300,400,500,700&display=swap');

  * {
    box-sizing: border-box;
  }

  h1, h2, h3, h4, h5 {
    font-family: 'Roboto', sans-serif;
  }

  p, span, div, ul, a {
    font-family: 'Open Sans', sans-serif;
  }

  body {
    margin: 0;
  }

  .page {
    width: 100%;
    height: 100vh;
    display: flex;

    &__menu {
      width: 300px;
      border-right: 1px solid #d8d8d8;

      &__logo {
        border-bottom: 1px solid #d8d8d8;

        h1 {
          margin: 0;
          font-size: 19px;
          text-align: center;
          padding: 12px 0px;
        }
      }

      ul {
        margin: 0;
        padding: 0;
        list-style: none;

        > li {
          margin-top: 15px;
        }

        li {
          a {
            color: black;
            display: flex;
            padding-left: 25px;
          }

          ul {
            margin-left: 20px;
            li {
              a {
                text-decoration: none;
              }
            }
          }
        }
      }
    }

    &__content {
      width: 100%;
      padding: 10px 30px;

      &__text {

      }
    }
  }
</style>
