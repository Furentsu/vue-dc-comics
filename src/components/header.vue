<template>
  <div>
        <header>
            <div class="general-container">
                <a href="#" id="logo"><img src="../assets/img/dc-logo.png" alt="DC's logo"></a>
                

                <nav>
                    <ul>
                        <li v-for="(menu, index) in menu" :key="index">
                                <a href="#">{{menu.text}}</a>
                            </li>
                    </ul>
                </nav>
            </div>
          
        </header>
  </div>
</template>

<script>
export default {
    name: 'header',
    data: function() {
        return {
            menu: [
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
                    text: "Collectibles",
                },
                {
                    text: "Videos",
                },
                {
                    text: "Fans",
                },
                {
                    text: "News",
                },
                {
                    text: "Shop",
                }  
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

header { 
    height: 130px;

    .general-container {
        display: flex;
        align-items: center;
        height: 100%;
        justify-content: space-between;

        #logo {
            img {
                width: 80px;
            }
        }

        nav {
            height: 100%;
        }

        ul {
            display: flex;
            align-items: center;
            height: 100%;
            list-style: none;

            li {
                display: flex;
                align-items: stretch;
                height: 100%;
                font-size: 1rem;
                text-transform: uppercase;
                padding: 0 10px;
            }

                a {
                    display: flex;
                    align-items: center;
                    text-decoration: none;
                    border-bottom: 5px solid transparent;
                    color: $primaryBlack;

                    &:hover {
                        border-bottom: 5px solid $primaryBlue;
                    }

                }
        }
    }
}


</style>