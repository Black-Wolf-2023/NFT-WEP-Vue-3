<template lang="">
    <div id="Sell">
        <section id="sell" class="container">
            <h1>Create and sell your NFTs</h1>
            <div class="card-parent">
                <div class="sell-card">
                    <div class="cont-icon">
                        <img src="../../assets/Icons/monitor.svg" alt="" width="35px" height="35px">
                    </div>
                    <span>Set up your wallet</span>
                    <p>
                        Once you’ve set up your wallet of choice, connect it to OpenSea by clicking the
                        wallet icon in the top right corner.
                    </p>
                </div>
                <!-- ------- Card-1 -->
                <div class="sell-card">
                    <div class="cont-icon">
                        <img src="../../assets/Icons/monitor.svg" alt="" width="35px" height="35px">
                    </div>
                    <span>Add your NFTs</span>
                    <p>
                        Once you’ve set up your wallet of choice, connect it to OpenSea by clicking the
                        wallet icon in the top right corner.
                    </p>
                </div>
                <!-- ------- Card-2 -->
                <div class="sell-card">
                    <div class="cont-icon">
                        <img src="../../assets/Icons/monitor.svg" alt="" width="35px" height="35px">
                    </div>
                    <span>List them for sale</span>
                    <p>
                        Once you’ve set up your wallet of choice, connect it to OpenSea by clicking the
                        wallet icon in the top right corner.
                    </p>
                </div>
                <!-- ------- Card-3 -->
            </div>
        </section>
    </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
@import "../../sass/main";
#sell {
  text-align: center;
  h1 {
    font-size: 2.5rem;
    color: $white-color;
    margin-top: 80px;
    margin-bottom: 50px;
  }
  .card-parent {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
    .sell-card {
      @include flex(center, center, column, 40px);
      text-align: center;
      gap: 30px;
      background-color: $card-color;
      border-radius: 10px;
      border: 1px solid $white-color;
      &:hover {
        transform: translateY(-50px);
        cursor: pointer;
        background-color: transparent;
      }
      span {
        font-size: 1.5rem;
      }
      .cont-icon {
        width: 70px;
        height: 70px;
        background-color: $main-color;
        border-radius: 50%;
        @include flex(center, center, column, 0px);
      }
      @include media(em) {
        transform: scale(0.8);
        &:hover {
          transform: translateY(-50px) scale(0.8);
          cursor: pointer;
          background-color: transparent;
        }
      }
    }
    :nth-child(2) {
      background-color: transparent;
    }
    @include media(md) {
      grid-template-columns: 1fr 1fr;
    }
    @include media(sm) {
      grid-template-columns: 1fr 1fr;
    }
    @include media(em) {
      grid-template-columns: 1fr;
    }
  }
}
@include media(em) {
  #sell h1 {
    font-size: 1.5rem !important;
  }
}
</style>