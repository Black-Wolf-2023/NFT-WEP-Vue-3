<template lang="">
    <div id="Feature">
         <section id="featured" class="container">
            <div class="header-title">
                <h1>Authors</h1>
                <button class="nav-btn">View More</button>
            </div>
            <div class="elements">
                <div class="ele-cont">
                    <div class="img">
                        <img src="../../assets/Main/ft-per-1.png" alt="">
                    </div>
                    <span>Crispin Berry</span>
                    <div class="text">
                        <img src="../../assets/Icons/bit.svg" alt="">
                        <p>214.2 ETH</p>
                    </div>
                </div>
                <!-- ======== Ele-1 -->
                <div class="ele-cont">
                    <div class="img">
                        <img src="../../assets/Main/ft-per-2.png" alt="">
                    </div>
                    <span>Crispin Berry</span>
                    <div class="text">
                        <img src="../../assets/Icons/bit.svg" alt="">
                        <p>214.2 ETH</p>
                    </div>
                </div>
                <!-- ======== Ele-2 -->
                <div class="ele-cont">
                    <div class="img">
                        <img src="../../assets/Main/ft-per-3.png" alt="">
                    </div>
                    <span>Crispin Berry</span>
                    <div class="text">
                        <img src="../../assets/Icons/bit.svg" alt="">
                        <p>214.2 ETH</p>
                    </div>
                </div>
                <!-- ======== Ele-3 -->
                <div class="ele-cont">
                    <div class="img">
                        <img src="../../assets/Main/ft-per-4.png" alt="">
                    </div>
                    <span>Crispin Berry</span>
                    <div class="text">
                        <img src="../../assets/Icons/bit.svg" alt="">
                        <p>214.2 ETH</p>
                    </div>
                </div>
                <!-- ======== Ele-4 -->
                <div class="ele-cont">
                    <div class="img">
                        <img src="../../assets/Main/ft-per-5.png" alt="">
                    </div>
                    <span>Crispin Berry</span>
                    <div class="text">
                        <img src="../../assets/Icons/bit.svg" alt="">
                        <p>214.2 ETH</p>
                    </div>
                </div>
                <!-- ======== Ele-5 -->
                <div class="ele-cont">
                    <div class="img">
                        <img src="../../assets/Main/ft-per-6.png" alt="">
                    </div>
                    <span>Crispin Berry</span>
                    <div class="text">
                        <img src="../../assets/Icons/bit.svg" alt="">
                        <p>214.2 ETH</p>
                    </div>
                </div>
                <!-- ======== Ele-6 -->
            </div>
        </section>
    </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
@import "../../sass/main";
#featured {
  .elements {
    display: grid;
    grid-template-columns: repeat(6, 1fr);
    @include media(sm) {
      grid-template-columns: repeat(3, 1fr);
      gap: 50px;
    }
    @include media(em) {
      grid-template-columns: repeat(2, 1fr);
      gap: 50px;
    }
    .ele-cont {
      @include flex(center, flex-start, column, 0);
      gap: 10px;
      .img {
        width: 100px;
        height: 100px;
        &:hover {
          animation: cir 1s ease-out alternate forwards;
          cursor: pointer;
        }
      }
      .text {
        display: flex;
        img {
          width: 20px;
          height: 20px;
          margin-right: 10px;
        }
      }
    }
  }
}
@keyframes cir {
  from {
    transform: scale(0.9) rotate(360deg);
  }
  to {
    transform: scale(1.3) rotate(0deg);
  }
}
</style>