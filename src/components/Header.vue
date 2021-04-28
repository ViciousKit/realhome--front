<template>
  <nav class="navbar navbar-expand-lg navbar-light">
  <div class="container">
    <a class="navbar-brand logo" href="/"><img src="../assets/img/realhome_logo.png" alt=""></a>
    
    <div class="collapse collapse-fontsize navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-lg-0">
        <li class="nav-item" v-for="(menu, index) in headerMenuList" :key="index">
          <router-link class="nav-link active" aria-current="page" :to="menu.path">
            {{menu.name}}
            </router-link>
        </li>
      </ul>
      <div class="icons">
        <a href="#"><img src="../assets/img/icons/f.png" alt=""></a> 
        <a href="#"><img src="../assets/img/icons/p.png" alt=""></a>
        <a href="#"><img src="../assets/img/icons/inst.png" alt=""></a>
        <a href="#"><img src="../assets/img/icons/gmail.png" alt=""></a>
      </div>
    </div>
  </div>
</nav>
</template>

<script>
import {menuList} from '../constants/menuLinks.js';
export default {
  props: {
    msg: String
  },
  data() {
    return {
      headerMenuList: menuList
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .navbar-brand {
    color: red;
  }
  .container {
    height: 100%;
  }
  .navbar {
    padding: 0;
    height: 80px;
  }
  .logo {
    padding-right: 180px;
  }
  .collapse {
    margin: 0;
    padding: 0;
    height: 100%;
  }
  .collapse-fontsize {
    font-size: 18px;
  }
  
  .nav-link.active {
    padding: 30px 20px;
    height: 100%;
    &:hover {
      background: #f2f2f2;
    }
  }
  .icons {
    text-align: center;
    a {
      width: 30px;
      height: 30px;
      border: 1px solid #f2f2f2;
      border-radius: 50%;
      margin-right: 10px;
      display: inline-block;
    }
  }
</style>
