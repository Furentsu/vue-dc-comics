<template>
  <div>
      <header>
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
    display: flex;
    justify-content: space-around;
    align-items: center;
    padding: 20px;
    border: 1px solid red; // Debug !!
}

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
</style>