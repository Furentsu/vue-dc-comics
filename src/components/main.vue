<template>
  <div>
      <main>
          <div class="general-container">
              <h1>Content goes here</h1>
          </div>
      </main>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

main {
    background-color: $primaryBlack;
    height: 150px;

    .general-container {
        display: flex;
        align-items: center;
        height: 100%;
        color: $primaryWhite;

        h1 {
            font-size: 2rem;
        }
    }
}
</style>