<template>
    <div>
        <h1>layout</h1>
        <navMenu></navMenu>
        <sideBar></sideBar>
        <appMain></appMain>
    </div>
</template>
<script>
// import { navMenu, sideBar,appMain } from "./components/;
import {navMenu} from './components/navMenu.vue'
export default {
  name: "layout",
  components: {
    AppMain,
    NavMenu,
    SideBar
  },
  data() {
    return {};
  }
};
</script>
<style>
</style>


