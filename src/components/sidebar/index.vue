<template>
  <div class="sidebar-container">
    <div class="logo">
      <img alt="Logo" src="../../assets/logo.png">
    </div>
    <div class="sidebar-content">
      <div class="sidebar-menu-content">
        <div class="sidebar-menu-item" v-for="menuItem in sideMenu" :key="menuItem.name">
          <img class="sidebar-menu-icon" :alt="menuItem.name" :src="menuItem.icon">
          {{menuItem.name}}
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  import sideMenu from './sidemenu.config'
  export default {
    name: 'SideBar',
    props: {
        
    },
    data() {
      return {
        sideMenu
      }
    }
  }
</script>

<style>
  .sidebar-container {
    padding: 48px 20px 20px 20px;
    border: 1px solid rgba(228, 228, 228, 0.1);
  }

  .logo {
    width: 178px;
    height: 32px;
    margin-bottom: 44px;
  }

  .sidebar-content {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }

  .sidebar-menu-content {
    display: flex;
    flex-direction: column;
  }

  .sidebar-menu-item {
    display: flex;
    align-items: center;
    color: #777E90;
    padding: 16px 20px;
    border-radius: 8px;
    cursor: pointer;
  }

  .sidebar-menu-item:hover {
    background-color: #31343F;
    color: #EBCD81;
  }

  .sidebar-menu-icon {
    margin-right: 20px;
  }
</style>