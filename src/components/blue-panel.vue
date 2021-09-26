<template>
  <div>
      <section>
            <div class="general-container">
              <div class="content" v-for="(element, index) in panelContent" :key="index">
                  <img :src="element.image" :alt="element.alt">
                  <h3>{{element.text}}</h3>
              </div>
            </div>
      </section>
  </div>
</template>

<script>
export default {
    name:"blue-panel",
    data: function() { 
        return {
            panelContent: [
                {
                    image: require('../assets/img/buy-comics-digital-comics.png'),
                    alt: "Digital comics",
                    text: "Digital Comics"
                },
                {
                    image: require('../assets/img/buy-comics-merchandise.png'),
                    alt: "DC merchandise",
                    text: "DC merchandise"
                },
                {
                    image: require('../assets/img/buy-comics-subscriptions.png'),
                    alt: "Subscription",
                    text: "Subscription"
                },
                {
                    image: require('../assets/img/buy-comics-shop-locator.png'),
                    alt: "Comic shop locator",
                    text: "Comic shop locator"
                },
                {
                    image: require('../assets/img/buy-dc-power-visa.svg'),
                    alt: "DC power visa",
                    text: "DC power visa"
                },
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

section {
    background-color: $primaryBlue;
    height: 150px;

    .general-container {
        display: flex;
        justify-content: space-around;
        height: 100%;

        .content {
            display: flex;
            justify-content: space-between;
            color: $primaryWhite;
            align-items: center;

            img {
                width: 38px;
            }

            h3 {
                font-size: 1rem;
                padding: 0 25px;
                text-transform: uppercase;
            }
        }
    }
}
</style>