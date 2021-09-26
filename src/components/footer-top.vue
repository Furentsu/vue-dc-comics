<template>
  <div>
      <footer>
          <div class="general-container">
              <div class="footer-left">
                  <div class="footer-list-left">
                        <h2>DC COMICS</h2>
                        <ul>
                            <li v-for="(link, index) in dcComics" :key="index">
                                <a href="#">{{link.text}}</a>
                            </li>
                            
                        </ul>
                        <h2>SHOP</h2>
                        <ul>
                            <li v-for="(link, index) in shopDc" :key="index">
                                <a href="#">{{link.text}}</a>
                            </li>
                            
                        </ul>  
                  </div>

                  <div class="footer-list-center">
                        <h2>DC</h2>
                        <ul>
                            <li v-for="(link, index) in dc" :key="index">
                                <a href="#">{{link.text}}</a>
                            </li>
                            
                        </ul>
                  </div>

                  <div class="footer-list-right">
                        <h2>SITES</h2>
                        <ul>
                            <li v-for="(link, index) in sites" :key="index">
                                <a href="#">{{link.text}}</a>
                            </li>
                            
                        </ul>
                  </div>
              </div>
              <div class="footer-right">
                  <img src="../assets/img/dc-logo-bg.png" alt="DC logo">
              </div>
          </div>
      </footer>
  </div>
</template>

<script>
export default {
    name:'footer-op',
    data: function() { 
        return {
            dcComics: [
                {
                    text: "Characters",
                },
                {
                    text: "Comics",
                },
                {
                    text: "Movies",
                },
                {
                    text: "TV",
                },
                {
                    text: "Games",
                },
                {
                    text: "Videos",
                },
                {
                    text: "News",
                }
            ],

            shopDc: [
                {
                    text: "Shop DC",
                },
                {
                    text: "Shop DC Collectibles",
                }
            ],

            dc: [
                {
                    text: "Terms of use",
                },
                {
                    text: "Privacy policy (New)",
                },
                {
                    text: "Ad Choices",
                },
                {
                    text: "Advertising",
                },
                {
                    text: "Jobs",
                },
                {
                    text: "Subscriptions",
                },
                {
                    text: "Talent Workshops",
                },
                {
                    text: "CPSC Certificates",
                },
                {
                    text: "Ratings",
                },
                {
                    text: "Shop Help",
                },
                {
                    text: "Contact Us",
                }
            ],

            sites: [
                {
                    text: "DC",
                },
                {
                    text: "Mad Magazine",
                },
                {
                    text: "DC Kids",
                },
                {
                    text: "DC Universe",
                },
                {
                    text: "DC Power Visa",
                }
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

footer {
    height: 450px;
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: cover;

    .general-container {
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 100%;
        overflow: hidden;

        .footer-left {
            height: 100%;
            display: flex;
            justify-content: start;

            .footer-list-left,
            .footer-list-right,
            .footer-list-center {
                height: 100%;
                padding: 30px 20px;
            }
            
            h2 {
                color: $primaryWhite;
                text-transform: uppercase;
                padding: 18px 0;
                
            }

            ul {
                list-style: none;

                li {
                    font-size: 1rem;
                    padding: 5px 0;
                }

                    a {
                        text-decoration: none;
                        color: $secondaryGrey;
                    }
            }
        }
        
        .footer-right img {
            width: 80%;
        }

    }
}

</style>