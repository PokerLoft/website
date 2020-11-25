<template>
    <div class="nav-bar">
        <router-link to="/" class="name">
            <img class = "logo" src="../imgs/pokerloft.png"/>
            <span>Poker</span>
            <span style='color: #59BFFF;'>Loft</span>
        </router-link>
        <ul class="nav-links">
            <li>
                <router-link to="/sponsors" class="item">Sponsors</router-link>
            </li>
            <li>
                <a href="mailto:kev2018@mit.edu" class="item">Contact Us</a>
            </li>
            <li>
                <router-link to="/login" class="login" tag="button">Join</router-link>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
  name: "NavBar"
};
</script>

<style scoped>
.nav-bar {
    position: fixed;
    left: 0;
    top: 0;
    background: white;
    width: 100%;
    height: 4rem;
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.05);
    display: flex;
    justify-content: space-between;
    align-content: center;
    margin: 0;
    z-index: 10;
}

.logo {
    width: 40px;
    margin-right: 0.6rem;
}

.name {
    font-family: "Montserrat";
    font-style: normal;
    font-weight: 700;
    font-size: 24px;
    text-decoration: none;
    color: black;
    height: 100%;
    margin-left: 2rem;
    display: flex;
    align-items: center;
}

.nav-links {
    list-style: none;
    font-family: "Montserrat";
    font-style: normal;
    font-weight: 200;
    font-size: 18px;
    display: flex;
    text-align: center;
    justify-content: space-between;
    align-items: center;
    height: 100%;
    margin: 0;
}

.nav-links li {
    height: 3rem;
    display: flex;
    align-items: center;
}

.item {
    text-decoration: none;
    color: black;
    margin: 0 1rem;
}

.item:hover {
    text-decoration: underline;
}

.login {
    margin-left: 1rem;
    margin-right: 2rem;
    cursor: pointer;
    font-family: "Varela";
    font-style: normal;
    font-weight: 600;
    font-size: 18px;
    background-color: #59BFFF;
    filter: drop-shadow(0px 4px 4px rgba(0, 0, 0, 0.25));
    border: transparent;
    border-radius: 10px;
    padding: 8px 16px;
    width: 8rem;
    text-align: center;
    text-decoration: none;
    color: white;
}

.login:hover {
    opacity: 0.8;
    color: white;
}
</style>