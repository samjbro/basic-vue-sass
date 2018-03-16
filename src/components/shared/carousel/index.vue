<template>
    <div class="carousel" v-cloak>
        <div class="carousel__arrow carousel__arrow--left">
            <a href="#gallery-1">
                &lang;
            </a>
        </div>
        <div class="carousel__gallery carousel__gallery--1" id="gallery-1">
            <div class="row">
                <div class="col-1-of-3">
                    <img src="./sew-2.jpg" alt="Magazine Cover" class="carousel__img">
                </div>
                <div class="col-1-of-3">
                    <img src="./images/sew-3.jpg" alt="Magazine Cover" class="carousel__img">
                </div>
                <div class="col-1-of-3">
                    <img src="./images/sew-4.jpg" alt="Magazine Cover" class="carousel__img">
                </div>
            </div>
        </div>
        <div class="carousel__gallery carousel__gallery--2" id="gallery-2">
            <div class="row">
                <div class="col-1-of-3">
                    <img src="./images/sew-5.jpg" alt="Magazine Cover" class="carousel__img">
                </div>
                <div class="col-1-of-3">
                    <img src="./images/sew-6.jpg" alt="Magazine Cover" class="carousel__img">
                </div>
                <div class="col-1-of-3">
                    <img src="./images/sew-7.jpg" alt="Magazine Cover" class="carousel__img">
                </div>
            </div>
        </div>
        <div class="carousel__arrow carousel__arrow--right">
            <a href="#gallery-2">
                &rang;
            </a>
        </div>
    </div>
</template>

<script>

</script>

<style lang="scss">
    @import "~#/abstracts/variables";

    .carousel {
        text-align: center;
        position: relative;
        height: 38rem;

        &__arrow {
            font-size: 5rem;
            line-height: 5rem;
            display: inline-block;
            position: absolute;
            top: 50%;
            transform: translateY(-50%);

            a {
                text-decoration: none;
                color: inherit;
            }

            &--left {
                left: 0;
            }
            &--right {
                right: 0;
            }
        }

        &__gallery {
            display: inline-block;
            width: 80%;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            transition: all 1s;

            &--1 {
            }

            &--2 {
            }

            &:target {
                //transform:
            }

            &:not(:target) {
                transform: translate(-200%, -50%);
            }

        }

        &__img {
            width: 80%;
            box-shadow: 2rem 2rem 4rem rgba($color-black, .5);
        }
    }
</style>