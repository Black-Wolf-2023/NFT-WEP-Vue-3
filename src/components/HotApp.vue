<template lang="">
    <div id="Hot">
        
        <section id="hot" class="container">
            <div class="header-title">
                <h1>Live Actions</h1>
            </div>
            <div class="filter">
                <div @click="Activer(index)" class="cont" v-for="(item,index) in list" :key="item" :class="{'activer-cont': index == active}">{{item}}</div>
            </div>
            <div class="hot-cards">
                <div class="card">
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
                            <div class="bg-user"><img src="../../assets/Main/card-user-8.png" alt=""></div>
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
                <!-- =========== Card-1 -->
                <div class="card">
                    <div class="bg-img">
                        <img src="../../assets/Main/card-5.png" alt="">
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
                            <div class="bg-user"><img src="../../assets/Main/card-user-5.png" alt=""></div>
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
                <!-- =========== Card-2 -->
                <div class="card">
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
                <!-- =========== Card-3 -->
                <div class="card">
                    <div class="bg-img">
                        <img src="../../assets/Main/card-8.png" alt="">
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
                            <div class="bg-user"><img src="../../assets/Main/card-user-12.png" alt=""></div>
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
                <!-- =========== Card-4 -->
                <div class="card">
                    <div class="bg-img">
                        <img src="../../assets/Main/card-3.png" alt="">
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
                            <div class="bg-user"><img src="../../assets/Main/card-user-11.png" alt=""></div>
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
                <!-- =========== Card-5 -->
                <div class="card">
                    <div class="bg-img">
                        <img src="../../assets/Main/card-7.png" alt="">
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
                            <div class="bg-user"><img src="../../assets/Main/card-user-10.png" alt=""></div>
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
                <!-- =========== Card-6 -->
            </div>
            <a href="../../src/docs/search.html" class="nav-btn" style="display: block;">View More</a>
        </section>
    </div>
</template>
<script>
export default {
    data() {
        return {
            list: ["🎷 Music", "🎨 Art", "🎳 Sports", "🤖 Virtual", "📹 Videos", "More..."],
            active:4
        }
    },
    methods: {
        Activer(index) {
            this.active = index;
        }
    }
};
</script>
<style lang="scss" scoped>
@import "../../sass/main";
#hot {
  @include flex(center, center, column, 0px);
  .header-title {
    justify-content: center;
  }
  .filter {
    @include flex(center, center, row, 0px);
    flex-wrap: wrap;
    gap: 10px;
    .cont {
      text-align: center;
      background-color: $hot-color;
      padding: 10px 30px;
      color: $white-color;
      font-weight: 500;
      border-radius: 5px;
      cursor: pointer;
    }
    .activer-cont {
      background-color: $main-color;
      box-shadow: 2px 2px 10px $main-color;
    }
  }
  .hot-cards {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    justify-items: center;
    padding: 60px 0;
    @include media(sm) {
      grid-template-columns: repeat(2, 1fr);
    }
    @include media(em) {
      grid-template-columns: repeat(1, 1fr);
    }
    .card {
      transform: scale(0.8);
      .bg-img {
        position: relative;
        overflow: hidden;
        &:hover::after,
        &:hover::before {
          opacity: 1;
          visibility: visible;
        }
        &:hover::before {
          top: 50%;
        }
        &::after {
          content: "";
          position: absolute;
          border-radius: 10px;
          top: 0;
          left: 0;
          width: 100%;
          height: 100%;
          background-color: transparent;
          z-index: 10;
          backdrop-filter: blur(10px);
          @include flex(center, center, row, 0px);
          opacity: 0;
          visibility: hidden;
        }
        &::before {
          content: "Place a bid";
          position: absolute;
          top: 70%;
          left: 50%;
          transform: translate(-50%, -50%);
          z-index: 11;
          color: $white-color;
          font-weight: 500;
          background-color: $main-color;
          padding: 15px 30px;
          border-radius: 5px;
          cursor: pointer;
          opacity: 0;
          visibility: hidden;
          transition-delay: 0.1s;
        }
      }
    }
  }
}
</style>