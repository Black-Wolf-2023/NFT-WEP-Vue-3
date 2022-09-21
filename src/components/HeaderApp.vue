<template lang="">
    <div id="header">
        <div class="container">
            <header>
                <nav>
                    <div class="logo"><img src="../../assets/Logo/logo.svg" alt=""></div>
                    <ul class="list" :class="{'shower':state.list_status}">
                        <li><a href="#" class="active">Home</a></li>
                        <li><a href="./src/docs/search.html" class="disapled">Discover</a></li>
                        <li><a href="./src/docs/product.html" class="disapled">Docs</a></li>
                        <li><a href="#" class="disapled">Blog</a></li>
                        <li><a href="#" class="disapled">About Us</a></li>
                        <li><a href="#" class="disapled">Contact Us</a></li>
                        <li><a href="#" class="list-logo"><img src="../../assets/Logo/logo.svg" alt="" width="50px"
                                    height="50px"></a></li>
                    </ul>
                    <button class="nav-btn">Wallet</button>
                    <div class="toggle" @click = "state.list_status = !state.list_status">
                        <span></span>
                        <span></span>
                        <span></span>
                    </div>
                </nav>
            </header>
        </div>
    </div>
</template>
<script>
    import { reactive } from 'vue';
export default {
    setup() {
        const state = reactive({
            list_status:false
        })

        return {
            state
        }
    }

};
</script>
<style lang="scss">
@import "../../sass/main";
header {
  nav {
    @include flex(center, flex-start, row, 0px);
    @include media(mdsmem) {
      & {
        @include flex(center, space-between, row, 0px);
      }
    }
    height: 100px;
    .list {
      @include flex(center, center, row, 0);
      flex-grow: 1;
      gap: 40px;
      .list-logo {
        display: none;
      }
      li {
        a {
          font-weight: 600;
          &:hover::after {
            width: 100%;
          }
          &:hover {
            color: $main-color;
          }
        }
      }

      @include media(mdsmem) {
        & {
          position: fixed;
          top: 0;
          left: -100%;
          height: 100%;
          width: 65%;
          overflow: hidden;
          @include flex(flex-start, flex-start, column, 20px);
          background-color: $hot-color;
          z-index: 100;
          padding-top: 30%;
          .list-logo {
            display: block;
            position: absolute;
            bottom: 5%;
            left: 2%;
            img {
              object-fit: contain;
            }
          }
          li {
            width: 100%;
            img {
              display: block;
            }
            a {
              width: 100%;
              display: block;
            }
            .active,
            .disapled {
              text-align: center;
              padding: 10px 0;
              border-radius: 5px;
              box-shadow: inset 0 0 10px $white-color;
              background-color: $main-color;
              color: $white-color;
            }
            .disapled {
              background-color: transparent;
              border: none;
              box-shadow: inset 0 0 10px $main-color;
              background-color: $white-color;
              color: $main-color;
            }
            .active::after {
              display: none;
            }
          }
        }
      }
    }
  }
}
</style>