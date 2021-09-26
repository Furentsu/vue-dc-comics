<template>
  <div>
      <footer>
          <div class="general-container">
              <div class="footer-left">
                  <button type="button">Sign-up Now!</button>
              </div>
              <div class="footer-right">
                  <h2>Follow us</h2>
                  <ul>
                      <li><a href="#"><img src="../assets/img/footer-facebook.png" alt="Facebook's logo"></a></li>
                      <li><a href="#"><img src="../assets/img/footer-twitter.png" alt="Twitter's logo"></a></li>
                      <li><a href="#"><img src="../assets/img/footer-youtube.png" alt="Youtube's logo"></a></li>
                      <li><a href="#"><img src="../assets/img/footer-pinterest.png" alt="Pinterest's logo"></a></li>
                      <li><a href="#"><img src="../assets/img/footer-periscope.png" alt="Periscope's logo"></a></li>
                  </ul>
              </div>
          </div>
      </footer>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

footer {
    width: 100%;
    height: 120px;
    background-color: $primaryGrey;

    .general-container {
        display: flex;
        align-items: center;
        height: 100%;
        justify-content: space-between;

        .footer-left{
            button {
                font-size: 1.2rem;
                padding: 12px;
                background-color: transparent;
                color: $primaryWhite;
                text-transform: uppercase;
                border: 3px solid $primaryBlue;
                transition: all 300ms, ease-in-out 300ms;

                &:hover {
                    cursor: pointer;
                    color: $primaryBlue;
                    border-color: $primaryWhite;
                }
            }
        }
        
        .footer-right {
            display: flex;
            justify-content: end;
            align-items: center;

            h2 {
                font-size: 1.3rem;
                color: $primaryBlue;
                padding: 0 10px;
                text-transform: uppercase;
            }

            ul {
                display: flex;
                list-style: none;

                li {
                    padding: 0 10px;

                    a {
                        text-decoration: none;

                        img {
                            transition: all 250ms, ease-in-out 250ms;
                            border: 1px solid transparent;

                            &:hover {
                                background-color: $primaryWhite;
                                border: 1px solid $primaryWhite;
                                border-radius: 2em;
                            }
                        }
                    }
                }
            }
        }
    }

}
</style>