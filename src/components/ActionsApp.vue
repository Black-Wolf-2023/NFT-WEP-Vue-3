<template lang="">
    <div id="Actions">
         <section id="actions" class="container">
            <div class="header-title">
                <h1>Live Actions</h1>
                <button class="nav-btn">View More</button>
            </div>
            <div class="content">
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
                            <div class="bg-user"><img src="../../assets/Main/card-user-7.png" alt=""></div>
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
                <!-- ======= Card-1 -->
                <div class="card">
                    <div class="bg-img">
                        <img src="../../assets/Main/card-2.png" alt="">
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
                            <div class="bg-user"><img src="../../assets/Main/card-user-3.png" alt=""></div>

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
                <!-- ======= Card-2 -->
                <div class="card">
                    <div class="bg-img">
                        <img src="../../assets/Main/card-1.png" alt="">
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
                            <div class="bg-user"><img src="../../assets/Main/card-user-4.png" alt=""></div>
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
                <!-- ======= Card-3 -->
            </div>
        </section>
    </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
@import "../../sass/main";
#actions {
  .content {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    @include media(md) {
      grid-template-columns: 1fr 1fr;
    }
    @include media(sm) {
      grid-template-columns: 1fr 1fr;
      gap: 10px;
    }
    @include media(em) {
      grid-template-columns: 1fr;
    }
  }
}
</style>