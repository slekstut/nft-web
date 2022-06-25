<template>
    <div class="invitation-component wrapper">
        <div class="invitation-component__content">
            <h2>Create and sell your own NFTs</h2>
            <p>This roadmap outlines our goals and where we want to take Avatar Squad. We have a lot of ideas and
                concepts that we are working on. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
                tempor incididunt ut labore et. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
                tempor incididunt ut labore et.</p>
            <button>Sign up now</button>
        </div>
        <div class="invitation-component__images">
            <img src="../assets/images/contact-section-img2.png" alt="contact-section-img2.png">
            <img src="../assets/images/contact-section-img3.png" alt="contact-section-img3.png">
            <img src="../assets/images/contact-section-img1.png" alt="contact-section-img1.png">
        </div>
    </div>
</template>

<style lang="scss" scoped>
.invitation-component {
    padding-top: 178px;

    &__content {
        display: flex;
        flex-direction: column;
        align-items: start;

        h2 {
            max-width: 618px;
            font-weight: 400;
            font-size: 64px;
            line-height: 117.76%;
            margin-bottom: 20px;
        }

        p {
            max-width: 411px;
            font-weight: 400;
            font-size: 18px;
            line-height: 22px;
            margin-bottom: 40px;
        }

        button {
            padding: 15px 28px 14px 29px;
            font-weight: 400;
            font-size: 18px;
            line-height: 19px;
            color: $color-sand;
            background: $color-dark-blue;
            border-radius: 96px;
        }
    }

    &__images {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        // margin-top: -100px;
    }
}
</style>