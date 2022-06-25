<template>
    <div class="contact wrapper">
        <div class="contact__block">
            <h3>Let's get in touch</h3>
            <a href="mailto:hridoycraft @gmail.com">hridoycraft @gmail.com</a>
        </div>
    </div>
</template>

<script>
</script>

<style lang="scss" scoped>
.contact {
    display: flex;
    justify-content: center;
    align-items: center;

    .contact__block {
        min-width: 600px;
        padding: 40px;
        margin-top: 140px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        gap: 40px;
        background: #F0F0F0;
        box-shadow: 0px 4px 65px rgba(10, 13, 44, 0.05);
        border-radius: 286px;

        h3 {
            font-weight: 400;
            font-size: 48px;
            line-height: 117.76%;
        }

        a {
            font-weight: 400;
            font-size: 16px;
            line-height: 120%;
            position: relative;
            &::after {
                content: "";
                position: absolute;
                width: 100%;
                height: 1px;
                background-color: $color-dark-blue;
               bottom: -4px;
               left: 0;
            }
        }
    }
}
</style>