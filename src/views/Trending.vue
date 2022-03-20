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
      <div class="cards">
         <div class="arrows">
            <img src="../assets/images/arrow-left.svg" alt="arrow-left" class="arrow-left">
            <img src="../assets/images/arrow-right.svg" alt="arrow-right" class="arrow-right">
        </div>
        <div class="card">
          <div class="card__image">
            <img src="../assets/images/image-32.png" alt="image-32" />
          </div>
          <h3 class="card__title">Punk evelynn</h3>
          <p class="card__timing">24h : 24m : 24s</p>
          <a href="#" class="card__bid">Place a bid</a>
          <p class="card__price">245 ETH</p>
        </div>
        <div class="card">
          <div class="card__image">
            <img src="../assets/images/image-33.png" alt="image-33" />
          </div>
          <h3 class="card__title">Haslivbe</h3>
          <p class="card__timing">24h : 24m : 24s</p>
          <a href="#" class="card__bid">Place a bid</a>
          <p class="card__price">245 ETH</p>
        </div>
        <div class="card">
          <div class="card__image">
            <img src="../assets/images/image-34.png" alt="image-34" />
          </div>
          <h3 class="card__title">Prime Ape</h3>
          <p class="card__timing">24h : 24m : 24s</p>
          <a href="#" class="card__bid">Place a bid</a>
          <p class="card__price">245 ETH</p>
        </div>
        <div class="card">
          <div class="card__image">
            <img src="../assets/images/image-35.png" alt="image-35" />
          </div>
          <h3 class="card__title">KHALIFA</h3>
          <p class="card__timing">24h : 24m : 24s</p>
          <a href="#" class="card__bid">Place a bid</a>
          <p class="card__price">245 ETH</p>
        </div>
        <div class="card">
          <div class="card__image">
            <img src="../assets/images/image-36.png" alt="image-36" />
          </div>
          <h3 class="card__title">Futuristic Self</h3>
          <p class="card__timing">24h : 24m : 24s</p>
          <a href="#" class="card__bid">Place a bid</a>
          <p class="card__price">245 ETH</p>
        </div>
        <div class="card">
          <div class="card__image">
            <img src="../assets/images/image-37.png" alt="image-37" />
          </div>
          <h3 class="card__title">Voxel Nation</h3>
          <p class="card__timing">24h : 24m : 24s</p>
          <a href="#" class="card__bid">Place a bid</a>
          <p class="card__price">245 ETH</p>
        </div>
        <div class="vertical-lines">
            <img src="../assets/images/vertical-line.svg" alt="vertical-line" class="left-line">
            <img src="../assets/images/vertical-line.svg" alt="vertical-line" class="right-line">
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
    position: relative;
    padding: 0.625rem 1.0625rem;
    margin-top: 2.5rem;
    border: 2px solid $color-dark-blue;
    border-radius: 4rem;
    .filter-content {
      display: flex;
      flex-direction: row;
      gap: 4.375rem;
      button {
        width: fit-content;
        padding: 0;
        font-size: 1.125rem;
      }
      button.active-btn {
        padding: 11px 17px;
      }
    }
  }
  .cards {
    position: relative;
    width: 100%;
    margin-top: 6.25rem;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    column-gap: 3.5rem;
    row-gap: 6.875rem;
    .arrows {
            position: absolute;
            top: -5%;
            right: 0;
            transform: translate(0, 5%);
            display: flex;
            flex-direction: row;
            gap: 0.625rem;
        .arrow-left {
            
        }
        .arrow-right {
        }
    }
    .card {
      margin: 0 auto;
      place-items: center;
      & > * {
        text-align: center;
      }
      &__image {
        img {
          border-radius: 37.5rem;
        }
      }
      &__title {
        margin-top: 1rem;
        font-size: 2rem;
        line-height: 1.5;
      }
      &__timing {
        margin-top: 0.875rem;
        font-size: 1.125rem;
        opacity: 0.7;
      }
      &__bid {
        //margin-top: 0.875rem;
        display: block;
        font-size: 1.5rem;
        color: $color-dark-blue;
        text-align: center;
      }
      &__price {
        margin-top: 1rem;
        font-size: 1.5rem;
        font-weight: 700;
      }
    }
    .vertical-lines {
        .left-line {
            position: absolute;
            top: 0;
            left: 31%;
            transform: translateX(-31%);
        }
        .right-line {
            position: absolute;
            top: 0;
            right: 26%;
            transform: translateX(-26%);
        }
    }
  }
}
</style>
