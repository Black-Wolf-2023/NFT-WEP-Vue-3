<template lang="">
    <div id="Hero">
        <section id="hero" class="container">
            <div class="content">
                <div class="head">
                    <h1>Discover a New Era of Crypto Currency</h1>
                    <p>
                        Panda NFT is the primier marketplace for NFT, which are digital items you can
                        truly own. Digital items have existed for a long time, but never like this.</p>
                    <button class="nav-btn">Get Start</button>
                </div>
                <div class="cards">
                    <div class="card" :class="{'back-class':!slide.slide_status}">
                        <div class="bg-img">
                            <img src="../../assets/Main/card-4.png" alt="">
                            <div class="hot">
                                <div class="img">
                                    <img src="../../assets/Icons/001-fire.svg" alt="">
                                </div>
                                <span>05 : 12 : 07 : 45</span>
                            </div>
                        </div>
                        <div class="title">
                            <span>"Hamlet Contemplates ...</span>
                            <span>BSC</span>
                        </div>
                        <div class="user">
                            <div class="user-img">
                                <div class="bg-user"><img src="../../assets/Main/card-user-1.png" alt=""></div>
                                <div class="info">
                                    <p>Creator</p>
                                    <span>SalvadorDali</span>
                                </div>
                            </div>
                            <div class="price">
                                <p>Current Bid</p>
                                <span>4.89 eTH</span>
                            </div>
                        </div>
                    </div>
                    <!-- ========== Card-2 =========== -->
                    <div class="card" :class="{'back-class':slide.slide_status}">
                        <div class="bg-img">
                            <img src="../../assets/Main/card-6.png" alt="">
                            <div class="hot">
                                <div class="img">
                                    <img src="../../assets/Icons/001-fire.svg" alt="">
                                </div>
                                <span>05 : 12 : 07 : 45</span>
                            </div>
                        </div>
                        <div class="title">
                            <span>"Hamlet Contemplates ...</span>
                            <span>BSC</span>
                        </div>
                        <div class="user">
                            <div class="user-img">
                                <div class="bg-user"><img src="../../assets/Main/card-user-2.png" alt=""></div>
                                <div class="info">
                                    <p>Creator</p>
                                    <span>SalvadorDali</span>
                                </div>
                            </div>
                            <div class="price">
                                <p>Current Bid</p>
                                <span>4.89 eTH</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="loges">
                <img src="../../assets/Icons/logo-1.svg" alt="" width="30px" height="30px">
                <img src="../../assets/Icons/logo-2.svg" alt="" width="30px" height="30px">
                <img src="../../assets/Icons/logo-3.svg" alt="" width="30px" height="30px">
                <img src="../../assets/Icons/logo-4.svg" alt="" width="30px" height="30px">
                <img src="../../assets/Icons/logo-5.svg" alt="" width="30px" height="30px">
            </div>
        </section>
    </div>
</template>
<script>
import { reactive , onMounted} from 'vue';
export default {

    setup() {
        const slide = reactive({
            slide_status: false,
            item:1
        })


        onMounted(() => {
            setInterval(() => {
                slide.slide_status = !slide.slide_status;
            }, 5000);
        })


        return {
            slide
        }
    }
};
</script>
<style lang="scss">
@import "../../sass/main";
#hero {
  .content {
    padding-top: 80px;
    gap: 20px;
    .head {
      @include flex(flex-start, space-between, column, 0);
      padding-top: 80px;
      @include media(mdsmem) {
        padding-top: 0;
      }
      gap: 30px;
      h1 {
        color: $white-color;
        font-size: 2.6rem;
      }
      button {
        background-color: $main-color;
        color: $white-color;
        &:hover {
          background-color: transparent;
        }
      }
    }
    .cards {
      overflow: hidden;
      width: 100%;
      @include flex(flex-end, center, row, 0);
      position: relative;
      height: 500px;
      .card {
        position: absolute;
        z-index: 2;
        left: 0%;
        transform: scale(1);
        z-index: 2;
        opacity: 1;
        transition: all 0.5s ease-in-out, z-index 0s;
        @include media(em) {
          transform: scale(0.7);
        }
      }
      .back-class {
        left: 50%;
        transform: scale(0.6);
        z-index: 1;
        opacity: 0.8;
      }
    }
  }
  .loges {
    @include flex(center, flex-start, row, 0);
    @include media(xl) {
      overflow: hidden;
    }
    &::-webkit-scrollbar{
      width: 0;
    }
    height: 150px;
    overflow: auto;
    img {
      cursor: pointer;
      &:hover {
        transform: scale(1.3);
      }
    }
  }
}
</style>