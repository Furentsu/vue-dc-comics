<template>
  <div>
      <section>
            <div class="general-container">
                <ul>
                    <li v-for="(element, index) in panelContent" :key="index">
                        <a href="#">
                            <img :src="element.image" :alt="element.alt">
                            <h3>{{element.text}}</h3>
                        </a>
                    </li>
                </ul>
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
        justify-content: space-between;
        height: 100%;

        ul {
            display: flex;
            align-items: center;
            justify-content: space-evenly;
            width: 100%;
            height: 100%;
            list-style: none;

            li {
                display: flex;
                justify-content: space-between;
                color: $primaryWhite;
                align-items: center;

                a {
                    display: flex;
                    align-items: center;
                    text-decoration: none;
                    color: $primaryWhite;

                    img {
                        width: 40px;
                    }

                    h3 {
                        font-size: .9rem;
                        padding: 0 25px;
                        text-transform: uppercase;
                    }
                }
            }
        }

    }
}
</style>