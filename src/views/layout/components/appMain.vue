<template>
    <div>
        <div class="nav-menu">
            <NavMenu></NavMenu>
        </div>
        <div class="side-bar">
            <SideBar></SideBar>
        </div>
        <div class="main-container">
            <transition name="fade-transform" mode="out-in">
                <!-- or name="fade" -->
                <!-- <router-view :key="key"></router-view> -->
                <router-view />
            </transition>
        </div>

    </div>
</template>
<script>
import NavMenu from "./compoments/navMenu.vue";
import SideBar from "./compoments/sideBar.vue";
export default {
  name: "appMain",
  components: {
    NavMenu,
    SideBar
  },
  data() {
    return {};
  }
};
</script>
<style scoped>
.nav-menu {
  position: absolute;
  height: 40px;
  top: 0;
  background-color: red;
}
</style>


