<template>
    <div class="landing">
        <div class="left">
            <div>
                <h1 class="slogan">Ready to evolve your poker game<br>to a whole new level?</h1>
                <span class="slogan emphasis line1">Join us for an action-packed</span>
                <br>
                <span class="slogan emphasis line2">collegiate bootcamp!</span>
                <p class="info">Our vision is to elevate the collegiate poker scene by providing a study group for college students.</p>
            </div>
            <router-link to="/login" class="join" tag="button">Join Us</router-link>
        </div>
        <img class="right" src="../imgs/upgrade.png">
    </div>
</template>

<script>
export default {
  name: "LandingFirstPage"
};
</script>

<style scoped>
@keyframes type {
    0% {
      width: 0;
    }
    1% {
      opacity: 1;
    }
    99.9% {
      border-right: 0.05em solid #59BFFF;
    }
    100% {
      opacity: 1;
      border: none;
    }
}

@-webkit-keyframes type {
    0% {
      width: 0;
    }
    1% {
      opacity: 1;
    }
    99.9% {
      border-right: 0.05em solid #59BFFF;
    }
    100% {
      opacity: 1;
      border: none;
    }
}

@keyframes type2 {
    0% {
      width: 0;
    }
    1% {
      opacity: 1;
    }
    99.9% {
      border-right: 0.05em solid #59BFFF;
    }
    100% {
      opacity: 1;
    }
}

@-webkit-keyframes type2 {
    0% {
      width: 0;
    }
    1% {
      opacity: 1;
    }
    99.9% {
      border-right: 0.05em solid #59BFFF;
    }
    100% {
      opacity: 1;
    }
}

@keyframes blink {
    from, to { border-color: transparent }
    50% { border-color: #59BFFF; }
}

@-webkit-keyframes blink {
    from, to { border-color: transparent }
    50% { border-color: #59BFFF; }
}

@keyframes fadeInAnimation { 
    0% { 
        opacity: 0; 
    } 
    100% { 
        opacity: 1; 
     } 
} 

.landing {
    display: flex;
    justify-content: center;
    align-items: center;
    animation: fadeInAnimation ease 1s;
    animation-iteration-count: 1; 
    animation-fill-mode: forwards;
    margin-bottom: 6rem;
}

.left {
    margin-top: 8rem;
    margin-left: 4rem;
    display: flex;
    flex-direction: column;
    justify-content: center;
    height: 675px;
    width: fit-content;
}

.right {
    margin-top: 8rem;
    margin-right: 4rem;
}

.slogan {
    font-family: "Varela";
    font-style: normal;
    font-weight: normal;
    font-size: 52px;
    margin: 0;
}

.emphasis {
    display: flex;
    color: #59BFFF;
    white-space: nowrap;
    overflow: hidden;
    display: inline-block;
    border-right: 0.05em solid #59BFFF;
}

.line1 {
    width: 700px; /* manually set width */
    opacity: 0;
    -webkit-animation: type 1s steps(40, end);
    animation: type 1s steps(40, end);
    -webkit-animation-delay: 0.5s;
    animation-delay: 0.5s;
    -webkit-animation-fill-mode: forwards;
    animation-fill-mode: forwards;
}

.line2 {
    width: 525px; /* manually set width */
    opacity: 0;
    -webkit-animation: type2 0.7s steps(20, end), blink 1s step-end infinite;
    animation: type2 0.7s steps(20, end), blink 1s step-end infinite;
    -webkit-animation-delay: 1.5s;
    animation-delay: 1.5s;
    -webkit-animation-fill-mode: forwards;
    animation-fill-mode: forwards;
}

.info {
    font-family: "Varela";
    font-style: normal;
    font-weight: normal;
    font-size: 18px;
    color: rgba(0, 0, 0, 0.6);
    width: 25rem;
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