<template>
  <div>
      <footer>
          <div class="general-container">
              <div class="footer-left">
                  
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
        
        .footer-left,
        .footer-right {
            width: 50%;
        }

        .footer-right img {
            width: 80%;
        }

    }
}

</style>