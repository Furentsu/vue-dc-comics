<template>
  <div>
      <div id="jumbo">
          <div class="main-content-title">
              <h3>Current series</h3>
          </div>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

#jumbo {
    background-image: url("../assets/img/jumbotron.jpg");
    height: 420px;
    position: relative;

    .main-content-title {
        width: fit-content;
        font-size: 1.1rem;
        padding: 12px;
        background-color: $primaryBlue;
        color: $primaryWhite;
        text-transform: uppercase;

        position: absolute;
        top:395px;
        left: 200px
    }
}

</style>