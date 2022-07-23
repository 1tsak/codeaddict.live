<template>
  <div>
    <header>
      <div class="branding">Code<span>Addict</span></div>
      <div v-if="!mobile" class="nav">
        <ul>
          <router-link class="links" to="abc">Home</router-link>
          <router-link class="links" to="#">Portfolio</router-link>
          <router-link class="links" to="#">About</router-link>
          <router-link class="links" to="#">Contact</router-link>
        </ul>
      </div>
      <img
        v-else
        @click="toogleMobileNav"
        class="menu-ic"
        :src="menuIc"
        alt=""
      />
      <div class="toggle-mode">
        <i class="fas fa-moon"></i>
      </div>
    </header>
    <transition name="nav-mobile">
      <ul v-show="mobileNav" class="nav-mobile">
        <router-link class="links" to="abc">Home</router-link>
        <router-link class="links" to="#">Services</router-link>
        <router-link class="links" to="#">About</router-link>
        <router-link class="links" to="#">Contact</router-link>
      </ul>
    </transition>
  </div>
</template>

<script>
import menuIc from "@/assets/menu.svg";
export default {
  name: "NavBar",
  created() {
    window.addEventListener("resize", this.checkScreen);
    this.checkScreen();
  },
  setup() {
    return {
      menuIc,
    };
  },
  data() {
    return {
      mobile: null,
      mobileNav: null,
      windowWidth: null,
    };
  },
  methods: {
    checkScreen() {
      this.windowWidth = window.innerWidth;
      if (this.windowWidth <= 750) {
        this.mobile = true;
        return;
      }
      this.mobile = false;
      this.mobileNav = false;
      return;
    },
    toogleMobileNav() {
      this.mobileNav = !this.mobileNav;
    },
  },
};
</script>

<style lang="scss" scoped>
$pColor: #2290e8;
$sColor: #f34336;
header {
  display: flex;
  color: #36454f;
  justify-content: space-between;
  // box-shadow: 0 0 5px 0 rgba($color: #000000, $alpha: 0.3);
  align-items: center;
  margin: 0 auto;

  .branding {
    margin: 20px 25px;
    font-weight: 500;
    font-size: 20px;
    color: #36454f;
  }

  span {
    color: $sColor;
  }
  ul {
    margin-right: 25px;
  }
  .links {
    margin: 0px 15px;
    font-weight: 250;
    font-size: 1.0rem;
    // text-transform: uppercase;
    cursor: pointer;
    &:hover {
      border-bottom: 1px solid rgb(80, 87, 126);
    }
  }
}
.menu-ic {
  height: 22px;
  width: 22px;
  margin-right: 25px;
}
.nav-mobile {
  height: 100vh;
  width: 70%;
  background: #323232;
  position: absolute;
  top: 0;
  left: 0;
  display: flex;
  transition: 1s ease;
  flex-direction: column;
  max-width: 250px;

  .links {
    font-weight: 400;
    font-size: 20px;
    padding: 10px 25px;
    font-size: 16px;
    color: white !important;
    text-transform: uppercase;
    cursor: pointer;
  }
  .links:first-child {
    margin-top: 25px;
  }
}
.nav-mobile-enter-active,
.nav-mobile-leave-active {
  transition: all 1s ease;
}
.nav-mobile-enter-from {
  transform: translateX(-250px);
}
.nav-mobile-enter-to {
  transform: translateX(0);
}
.nav-mobile-leave-to {
  transform: translateX(-250px);
}
.toggle-mode {
  padding-right: 35px;
  padding-left: 25px;
}
</style>