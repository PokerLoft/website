<template>
    <div class="login">
        <Navbar/>
        <h1 class="info">We'll be starting <span style='color: #59BFFF;'> Season 1 </span> soon!</h1>
        <form action="mailto:kevin@npoint.ai" method="post" enctype="text/plain" class="apply-form">
            <div class="input">
                Email<br>
                <input type="text" name="mail" placeholder="example@email.com" class="field-input">
            </div>
            <input type="submit" value="Apply" class="apply">
        </form>
    </div>
</template>

<script>
import Navbar from "../components/Navbar.vue";

export default {
    name: "Login",
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

.login {
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

.apply-form {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-top: 2rem;
    animation: fadeInAnimation ease 2s;
    animation-iteration-count: 1; 
    animation-fill-mode: forwards;
}

.input {
    display: flex;
    flex-direction: column;
    justify-content: center;
    width: 600px;
    background: #FFFFFF;
    box-shadow: 0px 43px 50px 5px rgba(0, 0, 0, 0.1);
    border-radius: 15px;
    padding: 4rem 3rem;
    font-family: "Montserrat";
    font-style: normal;
    font-weight: 300;
    font-size: 14px;
}

.field-input {
    outline: 0;
    border-width: 0 0 2px;
    border-color: rgba(0, 0, 0, 0.1);
    font-family: "Montserrat";
    font-style: normal;
    font-weight: 500;
    font-size: 18px;
    margin-top: 0.25rem;
}

.field-input:focus {
    border-color: rgba(0, 0, 0, 0.7);
}

.apply {
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
}

.apply:hover {
    opacity: 0.8;
    color: white;
}
</style>
