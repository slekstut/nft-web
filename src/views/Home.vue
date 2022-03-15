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
          <div class="header-images">
            <div class="header-image">
              <img src="../assets/images/image-27.png" alt="image-27.png" />
            </div>
            <div class="header-image">
              <img src="../assets/images/image-30.png" alt="image-30.png" />
            </div>
            <div class="header-image">
              <img src="../assets/images/image-28.png" alt="image-28.png" />
            </div>
            <div class="header-image">
              <img src="../assets/images/image-29.png" alt="image-29.png" />
            </div>
          </div>
          <div class="img-separator"></div>
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
header {
  display: grid;
  gap: $gap-2;
  grid-template-columns: 1fr 1fr;
  justify-content: center;
  align-items: start;
  margin-top: 7rem;
  .header-left {
    display: grid;
    gap: $gap-2;
    grid-template-columns: 1fr;
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
      display: flex;
      flex-direction: row;
      justify-content: start;
      align-items: center;
    }
  }
  .header-right {
    position: relative;
    .header-images {
      display: grid;
      gap: $gap-2 0;
      grid-template-columns: 1fr 1fr;
      .header-image {
        img {
          border-radius: 9.8125rem;
          margin-left: auto;
        }
      }
    }
    .img-separator {
      width: 992px;
      height: 600px;
      background-image: url("../assets/images/separator.svg");
      background-position: center;
      background-repeat: no-repeat;
      background-size: cover;
      position: absolute;
      position: absolute;
      top: 50%;
      right: 0;
      transform: translateY(-50%);
      z-index: -1;
    }
  }
}
</style>
