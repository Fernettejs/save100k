<template>
    <section class="banner" id="home">
        <div class="textBox">
            <h1>Let's become wealthy together.</h1>
            <a href="#about" class="btn">Read More</a>
        </div>
    </section>
</template>

<style scoped>

.banner {
    position: relative;
    min-height: 100vh;
    background-image: url(../assets/money-seedling-b&w.png);
    background-size: cover;
    background-position: top;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.banner h1{
    font-size: 4em;
    color: #fff;
    text-shadow: -2px 2px#85bb65;
    font-weight: 700;
    line-height: 1.2em;
}

.banner h3 {
    font-size: 1.5em;
    color: #fff;
    font-weight: 500;
}

.btn{
    position: relative;
    background: #85bb65;
    display: inline-block;
    color: #fff;
    margin-top: 20px;
    padding: 10px 30px;
    font-size: 18px;
    text-transform: uppercase;
    text-decoration: none;
    letter-spacing: 2px;
    font-weight: 500;
}

</style>

<script>
export default {
    
}
</script>