<template>
  <div class="full-bleed">
    <div class="wrapper">
      <header>
        <h1>Trending auctions</h1>
        <p>
          The pain itself is love, the main storage system. It's not a great
          idea, it's a free and ugly scenario of life. And so that the curse
          should be a weekend even for. Coaching range
        </p>
      </header>
      <div class="filter-wrapper">
        <div class="filter-content">
          <button class="active-btn">Trending</button>
          <button>Art</button>
          <button>Ape</button>
          <button>Monkey</button>
          <button>Zombie</button>
          <button>Zombie</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.wrapper {
  margin-top: 6.25rem;
  display: grid;
  place-items: center;
  header {
    width: 100%;
    h1 {
      margin-bottom: 1.25rem;
      font-size: 4rem;
      line-height: 1.5;
      text-align: center;
    }
    p {
      width: 50%;
      margin: 0 auto;
      font-size: 1.125rem;
      text-align: center;
    }
  }
  .filter-wrapper {
    padding: 0.625rem 1.0625rem;
    margin-top: 2.5rem;
    border: 2px solid $color-dark-blue;
    border-radius: 4rem;
    .filter-content {
      display: flex;
      flex-direction: row;
      gap: 2rem;
      button {
        font-size: 1.125rem;
      }
    }
  }
}
</style>
