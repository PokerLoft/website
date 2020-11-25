<template>
    <div class="footer">
        <p class="copyright">© 2020 PokerLoft</p>
    </div>
</template>

<script>
export default {
    name: "Footer"
};
</script>

<style scoped>
.footer {
    display: flex;
    justify-content: center;
    width: 100%;
    height: 4rem;
    background: rgba(231, 231, 231, 0.25);
}

.copyright {
    font-family: Montserrat;
    font-style: normal;
    font-weight: 200;
    font-size: 14px;
    display: flex;
    align-items: center;
    text-align: center;
}
</style>