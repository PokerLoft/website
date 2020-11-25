<template>
    <div class="landing-two">
        <div class="even-cards">
            <FeatureCard v-for="(card, index) in evenCards" :key="index" :filename="card.filename" :title="card.title" :description="card.description"/>
        </div>
        <div class="odd-cards">
            <FeatureCard v-for="(card, index) in oddCards" :key="index" :filename="card.filename" :title="card.title" :description="card.description"/>
        </div>
    </div>
</template>

<script>
import FeatureCard from "./FeatureCard.vue";

export default {
    name: "LandingSecondPage",
    components: {
        FeatureCard
    },
    data() {
        return {
            cards: [
                {
                    filename: "chips.png",
                    title: "Enhance Your Edge",
                    description: "Whether you’re playing poker for the first time or already know\
                     PioSolver GTO solutions, the PokerLoft community is here to help you improve\
                     your game! During the bootcamp, you will have some of the best cash game and\
                     MTT courses in the world at your fingertips for you to study."
                },
                {
                    filename: "connections.png",
                    title: "Build Lasting Connections",
                    description: "PokerLoft puts the group in study group. Not only will you grind\
                     poker and battle the tables with your campmates, but you will also go on\
                     exciting adventures and have fun experiences together. In other words,\
                     work hard play hard."
                },
                {
                    filename: "lifestyle.png",
                    title: "Improve Your Lifestyle",
                    description: "Poker isn’t just a game of numbers. The processes of dealing with\
                     tilt, developing the disciplined mindset, and persevering through challenges\
                     are what separate good players from the great players. The lessons you learn\
                     at PokerLoft can be used in other aspects of life."
                }
            ]
        }
    },
    computed: {
        oddCards: function() {
            return this.cards.filter((_, i) => i % 2 === 1);
        },
        evenCards: function() {
            return this.cards.filter((_, i) => i % 2 === 0);
        }
    }
};
</script>

<style scoped>
.landing-two {
    width: 100%;
    height: 150%;
    display: flex;
    justify-content: center;
    overflow: hidden;
}

.even-cards {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    overflow: hidden;
}

.odd-cards {
    display: flex;
    align-items: center;
}

</style>