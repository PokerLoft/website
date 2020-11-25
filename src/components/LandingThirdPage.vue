<template>
    <div class="landing-third">
        <h1 class="title">Our Supporters</h1>
        <div class="supporter-logos">
            <img v-for="(name, index) in filenames" :key="index" :src="require(`../imgs/${name}`)" class="supporter"/>
        </div>
        <router-link to="/login" class="join" tag="button">Join Us</router-link>
    </div>
</template>

<script>
export default {
    name: "LandingThirdPage",
    data() {
        return {
            filenames: [
                'mpclogo.png'
            ]
        }
    }
};
</script>

<style scoped>
.landing-third {
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

.title {
    font-family: "Montserrat";
    font-style: normal;
    font-weight: bold;
    font-size: 36px;
}

.supporter-logos {
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 2rem 0;
}

.supporter {
    margin: 0 6rem;
}

.join {
    cursor: pointer;
    font-family: "Varela";
    font-style: normal;
    font-weight: 600;
    font-size: 24px;
    background-color: #59BFFF;
    filter: drop-shadow(0px 4px 4px rgba(0, 0, 0, 0.25));
    border: transparent;
    border-radius: 10px;
    padding: 20px 36px;
    width: 18rem;
    text-align: center;
    margin: 4rem 0;
    color: white;
    text-decoration: none;
}

.join:hover {
    opacity: 0.8;
    color: white;
}
</style>