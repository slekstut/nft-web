<template>
  <div class="full-bleed">
    <div class="wrapper">
      <router-link to="/">
        <div class="logo"></div>
      </router-link>
      <nav>
        <ul>
          <li><router-link to="/">Discover</router-link></li>
          <li><router-link to="/about">Marketplace</router-link></li>
          <li><router-link to="/about">Creator</router-link></li>
        </ul>
      </nav>
      <div class="mobile-menu">menu</div>
      <div class="cta">
        <button
          @click="isActiveBtn = !isActiveBtn"
          :class="[ isActiveBtn ? 'active-btn' : '' ]"
        >
          <router-link to="/">Login</router-link>
        </button>
        <button
          @click="isActiveBtn = !isActiveBtn"
          :class="[ !isActiveBtn ? 'active-btn' : '' ]"
        >
          <router-link to="/">Create wallet</router-link>
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isActiveBtn: false,
    };
  },
};
</script>

<style lang="scss" scoped>
.full-bleed {
  .wrapper {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 2.5rem;
    .logo {
      background-image: url("../assets/images/logo.png");
      background-position: center;
      background-repeat: no-repeat;
      background-size: cover;
      height: 43px;
      width: 85px;
    }
    nav ul {
      display: flex;
      gap: $gap-2;
      justify-content: center;
      list-style: none;
      li {
        a {
          font-size: 1rem;
          color: $color-dark-blue;
          text-decoration: none;
        }
      }
    }
    .mobile-menu {
      display: none;
    }
    .cta {
      display: flex;
      gap: 0.5rem;
    }
  }
}
</style>