<template>
    <div class="card">
        <div class="feature">
            <img :src="require(`../imgs/${filename}`)" class="feature-img">
            <h1 class="title">{{ title }}</h1>
        </div>
        <p class="description">{{ description }}</p>
    </div>
</template>

<script>
export default {
    name: "FeatureCard",
    props: ['filename', 'title', 'description']
};
</script>

<style scoped>
.card {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 575px;
    height: 475px;
    box-shadow: 0px 0px 20px 10px rgba(0, 0, 0, 0.1);
    border-radius: 15px;
    background: white;
    margin: 2rem 4rem 7rem 4rem;
}

.feature {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

.feature-img {
    width: 150px;
}

.title {
    font-family: "Montserrat";
    font-weight: 800;
    font-size: 24px;
    display: flex;
    align-items: center;
    text-align: center;
    margin: 2rem 0;
}

.description {
    font-family: "Montserrat";
    font-style: normal;
    font-weight: 300;
    font-size: 18px;
    display: flex;
    align-items: center;
    margin: 1rem 0;
    width: 450px;
}
</style>