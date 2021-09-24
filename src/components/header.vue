<template>
  <div>
        <header>
            <div class="general-container">
                <img src="../assets/img/dc-logo.png" alt="DC's logo">

                <nav>
                    <ul>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Comics</a></li>
                        <li><a href="#">Movies</a></li>
                        <li><a href="#">TV</a></li>
                        <li><a href="#">Games</a></li>
                        <li><a href="#">Collectibles</a></li>
                        <li><a href="#">Videos</a></li>
                        <li><a href="#">Fans</a></li>
                        <li><a href="#">News</a></li>
                        <li><a href="#">Shop</a></li>
                    </ul>
                </nav>
            </div>
          
        </header>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

header { 
    height: 150px;

    .general-container {
        display: flex;
        align-items: center;
        height: 100%;
        justify-content: space-between;

        ul {
            display: flex;
            list-style: none;

            li {
                font-size: 1rem;
                text-transform: uppercase;
                padding: 0 10px;
            }

                li a {
                    text-decoration: none;
                    color: $primaryBlack;
                }
        }
    }
}


</style>