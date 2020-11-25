<template>
    <div class="sponsors">
        <Navbar/>
        <h1 class="info">Join as a sponsor!</h1>
        <p class="benefits">As a sponsor, you will receive benefits including featuring sponsor swag, creating sponsor podcasts, advancing poker at the collegiate level, and meeting cool people!</p>
    </div>
</template>

<script>
import Navbar from "../components/Navbar.vue";

export default {
    name: "sponsors",
    components: {
        Navbar
    }
};
</script>

<style scoped>
@keyframes fadeInAnimation { 
    0% { 
        opacity: 0; 
    } 
    100% { 
        opacity: 1; 
     } 
} 

span {
    white-space:pre;
}

.sponsors {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 100%;
    margin-top: 8rem;
    animation: fadeInAnimation ease 1s;
    animation-iteration-count: 1; 
    animation-fill-mode: forwards;
}

.info {
    font-family: "Montserrat";
    font-style: normal;
    font-weight: bold;
    font-size: 48px;
    display: flex;
    align-items: center;
    text-align: center;
    margin: 2rem 0;
}

.benefits {
    font-family: "Montserrat";
    font-style: normal;
}
</style>
