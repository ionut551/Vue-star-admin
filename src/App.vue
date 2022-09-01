<template>
  <SideBar class="sidebar" />
  <main class="main">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </main>
</template>

<script>
import SideBar from './components/sidebar'
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    SideBar
  }
}
</script>

<style>
  @font-face {
    font-family: "Montserrat";
    src: url(fonts/OpenSans-Light.ttf);
    font-display: swap;
    font-weight: 300;
  }

  @font-face {
    font-family: "Montserrat";
    src: url(fonts/OpenSans-Regular.ttf);
    font-display: swap;
    font-weight: 400;
  }

  @font-face {
    font-family: "Montserrat";
    src: url(fonts/OpenSans-Medium.ttf);
    font-display: swap;
    font-weight: 500;
  }

  @font-face {
    font-family: "Montserrat";
    src: url(fonts/OpenSans-SemiBold.ttf);
    font-display: swap;
    font-weight: 600;
  }

  @font-face {
    font-family: "Montserrat";
    src: url(fonts/OpenSans-Bold.ttf);
    font-display: swap;
    font-weight: 700;
  }

  @font-face {
    font-family: "Montserrat";
    src: url(fonts/OpenSans-ExtraBold.ttf);
    font-display: swap;
    font-weight: 800;
  }

  #app {
    font-family: Montserrat, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    display: flex;
    width: 100%;
    background-color: #1F2128;
  }

  .sidebar {
    width: 256px;
  }

  .main {
    margin: 48px 64px 60px 64px;
  }
</style>
