<template>
  <div class="full-bleed">
    <div class="wrapper">
      <div class="number-box">
        <div class="number-box__content">
          <h3>20k+</h3>
          <p>Artwork</p>
        </div>
        <div class="number-box__content">
          <h3>15k</h3>
          <p>Auction</p>
        </div>
        <div class="number-box__content">
          <h3>8k</h3>
          <p>Artist</p>
        </div>
      </div>
      <div class="about-section">
        <div class="about-left">
          <img src="../assets/images/image31.png"/>
        </div>
        <div class="about-right">
          <div>
            <h1>Why we are different with others</h1>
            <p>The pain itself is love, the main storage system. It's not a great idea, it's a free and ugly scenario of life. And that is the curse of the weekend.</p>
            <button class="active-btn">Learn more</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "About"
}
</script>

<style lang="scss" scoped>
  .full-bleed {
    margin-top: 10rem;
    .wrapper {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      gap: $gap-3 + 7.375rem;
      .number-box {
        display: flex;
        flex-direction: row;
        justify-content: center;
        gap: $gap-3 + 2rem;
        width: fit-content;
        background-color: $color-white;
        border-radius: 11.8125rem;
        padding: 2.3125rem 7.25rem;
        &__content {
          h3 {
          font-size: 3rem;
          line-height: 1.2;
          font-weight: 400;
          }
          p {
            font-size: 1.5rem;
            font-weight: 400;
          }
        }
      }
      .about-section {
        display: grid;
        grid-template-columns: 1fr 1fr;
        .about-left {
          img {
            border-radius: 18.75rem;
          }
        }
        .about-right {
          display: flex;
          flex-direction: column;
          justify-content: center;
          align-items: center;
          gap: $gap-1;
          div {
            display: flex;
            flex-direction: column;
            gap: $gap-2;
          h1 {
            font-size: 3.8rem;
            font-weight: 400;
            color: $color-dark-blue;
            line-height: 1.4;
          }
          p {
            font-size: 1.125rem;
            max-width: 75%;
          }
          button {
            width: fit-content;
            color: $color-sand;
          }
          }
        }
      }
    }
  }
  
</style>
