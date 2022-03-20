<template>
  <div class="full-bleed">
    <div class="wrapper">
      <header>
        <div class="header-left">
          <h1>Keep calm & collect your NFTs</h1>
          <p>
            Lorem ipsum dolor sit amet consectetur adipiscing elit amet diam in
            est pharetra porttitor libero netus nulla tempor cont.
          </p>
          <div class="cta">
            <button
              @click="isActiveBtn = !isActiveBtn"
              :class="[!isActiveBtn ? 'active-btn' : '']"
            >
              <router-link to="/">Explore artwork</router-link>
            </button>
            <button
              @click="isActiveBtn = !isActiveBtn"
              :class="[isActiveBtn ? 'active-btn' : '']"
            >
              <router-link to="/">Create wallet</router-link>
            </button>
          </div>
        </div>
        <div class="header-right">
          <img src="../assets/images/header-img.png" />
        </div>
      </header>
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
.wrapper {
  margin-top: 5rem;
  header {
    display: flex;
    gap: $gap-2;
    flex-direction: row;
    justify-content: start;
    align-items: center;
    position: relative;
    .header-left {
      display: grid;
      gap: $gap-3;
      grid-template-columns: 1fr;
      margin-top: 8.5rem;
      width: 55%;
      h1 {
        font-size: 6rem;
        color: $color-dark-blue;
        font-weight: 700;
        line-height: 1;
      }
      p {
        font-size: 1.5rem;
        color: $color-dark-blue;
        opacity: 0.7;
        font-weight: 400;
        line-height: 1.3;
        max-width: 80%;
      }
      .cta {
        width: fit-content;
        display: flex;
        flex-direction: row;
        justify-content: start;
        align-items: center;
        button {
          padding: 1.1875rem 2rem;
        }
      }
    }
    .header-right {
      width: 100%;
      max-width: 992px;
      height: 700px;
      z-index: -1;
      position: absolute;
      bottom: -6%;
      right: 0;
      transform: translateY(6%);
      img {
        width: 100%;
        height: auto;
      }
    }
  }
}
</style>
