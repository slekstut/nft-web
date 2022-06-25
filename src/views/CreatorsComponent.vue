<template>
  <div class="full-bleed">
    <div class="wrapper">
      <section class="creators-text">
        <header>
          <h1>Creators</h1>
          <p>
            The pain itself is love, the main storage system. Not a great, free
            and disgraceful scenario of life
          </p>
        </header>
        <div class="creators-profiles">
          <div class="profile">
            <div class="profile__image">
              <img src="../assets/images/creator-1.png" alt="creator-1" />
            </div>
            <div class="profile__info">
              <h5>Hridoy</h5>
              <button>Follow</button>
            </div>
            <div class="profile__icons">
              <img src="../assets/images/mask1.png" alt="mask1" />
              <img src="../assets/images/mask2.png" alt="mask2" />
              <img src="../assets/images/mask3.png" alt="mask3" />
              <img src="../assets/images/mask4.png" alt="mask4" />
              <img src="../assets/images/mask5.png" alt="mask5" />
              <img src="../assets/images/mask6.png" alt="mask6" />
            </div>
          </div>
          <div class="profile">
            <div class="profile__image">
              <img src="../assets/images/creator-2.png" alt="creator-2" />
            </div>
            <div class="profile__info">
              <h5>Mita</h5>
              <button>Follow</button>
            </div>
            <div class="profile__icons">
              <img src="../assets/images/mask7.png" alt="mask7" />
              <img src="../assets/images/mask8.png" alt="mask8" />
              <img src="../assets/images/mask9.png" alt="mask9" />
              <img src="../assets/images/mask10.png" alt="mask10" />
              <img src="../assets/images/mask11.png" alt="mask11" />
              <img src="../assets/images/mask12.png" alt="mask12" />
            </div>
          </div>
        </div>
      </section>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.full-bleed {
  background-color: $color-dark-blue;
  .creators-text {
    display: grid;
    place-items: center;
    color: $color-sand;
    padding: 3.75rem 0;
    header {
      text-align: center;
      h1 {
        font-size: 4rem;
        margin-bottom: 1.25rem;
        font-weight: 400;
      }
      p {
        max-width: 50%;
        margin: 0 auto;
        font-size: 1.125rem;
        opacity: 0.7;
        font-weight: 400;
      }
    }
    .creators-profiles {
      display: flex;
      flex-direction: row;
      gap: 10rem;
      .profile {
        margin-top: 60px;
        &__image {
            position: relative;
            img {
            margin: 0 auto;
            }
        }
        &__image::after {
            position: absolute;
            content: '';
            width: 30px;
            height: 30px;
            bottom: 0;
            right: 37%;
            transform: translateX(-37%);
            background-color: $color-green;
            border-radius: 50%;
        }
        &__info {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin: 1.25rem 0;
            h5 {
                font-size: 2rem;
                margin: 0;
            }
            button {
                padding: 11px 24px;
                background-color: $color-sand;
                border-radius: 3rem;
            }
        }
        &__icons {
          display: flex;
          flex-wrap: wrap;
          justify-content: space-between;
          gap: 3.125rem;
          & img {
            flex: 0 0 25%;
          }
        }
      }
    }
  }
}
</style>
