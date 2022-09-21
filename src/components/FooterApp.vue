<template lang="">
    <div id="footer">
        <footer>
            <div class="header-title"></div>
            <div class="list-cont container">
                <ul>
                    <li><img src="../../assets/Logo/logo.svg" alt="" width="30px" height="30px"></li>
                    <li>
                        <p>
                            The world’s first and largest digital marketplace for crypto collectibles and non-fungible
                            tokens (NFTs). Buy, sell, and discover exclusive digital items.
                        </p>
                    </li>
                    <li class="copy-right">
                        <p>© 2022 by Abdalrhman Eldip ❤</p>
                    </li>
                </ul>
                <ul>
                    <li>
                        <h2>Resources</h2>
                    </li>
                    <li><a href="#">Help Center</a></li>
                    <li><a href="#">Platform Status</a></li>
                    <li><a href="#">Partners</a></li>
                    <li><a href="#">Gas-Free Marketplace</a></li>
                    <li><a href="#">Blog</a></li>
                </ul>
                <ul>
                    <li>
                        <h2>Company</h2>
                    </li>
                    <li><a href="#">Our Team</a></li>
                    <li><a href="#">About Us</a></li>
                    <li><a href="#">Contact Us</a></li>
                    <li><a href="#">Career</a></li>
                </ul>
                <ul>
                    <li>
                        <h2>Contact</h2>
                    </li>
                    <li><a href="#">2715 Ash Dr. San Jose, South Dakota 83475</a></li>
                    <li>
                        <div class="links">
                            <a href="#"><img src="../../assets/Icons/Facebook.svg" alt="" width="25px" height="25px"></a>
                            <a href="#"><img src="../../assets/Icons/twitter.svg" alt="" width="25px" height="25px"></a>
                            <a href="#"><img src="../../assets/Icons/instagram.svg" alt="" width="25px" height="25px"></a>
                        </div>
                    </li>
                </ul>
            </div>
        </footer>
    </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
@import "../../sass/main";
footer {
  padding-bottom: 70px;
  .list-cont {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    justify-items: center;
    @include media(sm) {
      grid-template-columns: repeat(2, 1fr);
      justify-items: flex-start;

      gap: 50px;
      :nth-child(1) {
        grid-row: 2/2;
      }
    }
    @include media(em) {
      grid-template-columns: repeat(1, 1fr);
      justify-items: flex-start;
      gap: 50px;
      :nth-child(1) {
        grid-row: 4/4;
      }
    }
    ul {
      @include flex(flex-start, flex-start, column, 0);
      gap: 20px;
      li {
        h2 {
          color: $white-color;
        }
        a {
          font-size: 14px;
          color: $light-color;
          font-weight: 500;
          &:hover {
            color: $main-color;
          }
        }
        .links {
          @include flex(center, center, row, 0);
          gap: 30px;
          a {
            @include flex(center, center, row, 0);
            background-color: $white-color;
            width: 35px;
            height: 35px;
            border-radius: 50%;
            &:hover {
              background-color: $main-color;
            }
          }
          :nth-child(2) {
            background-color: $main-color;
            &:hover {
              background-color: $hot-color;
            }
          }
        }
      }
      .copy-right {
        margin-top: 50px;
      }
    }
  }
}
</style>