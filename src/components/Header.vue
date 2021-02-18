<template>
    <header>
        <a href="#home" class="logo">Save 100k</a>
        <button class="cta-btn">Save </button>
        <div class="toggle" onclick="toggleMenu();"></div>
        <ul class="menu">
            <li><a href="#home" onclick="toggleMenu();">Home</a></li>
            <li><a href="#about" onclick="toggleMenu();">About</a></li>
            <li><a href="#contact" onclick="toggleMenu();">Contact</a></li>
        </ul>
    </header>
</template>

<style scoped>
header{
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    padding: 40px 100px;
    z-index: 1000;    
    display: flex;
    justify-content: space-between;
    align-items: center;
    transition: 0.5s;
}

header.sticky{
    background: #fff;
    padding: 20px 100px;
    box-shadow: 0 5px 20px rgba(0,0,0,0,0.1);
}
header .logo{
    color: #fff;
    font-size: 24px;
    text-transform: uppercase;
    text-decoration: none;
    font-weight: 700;
    letter-spacing: 2px;
}
header.sticky .logo{
    color: #111;
}
header ul{
    position: relative;
    display: flex;
}

header ul li{
    position: relative;
    list-style: none;
}
header ul li a{
    position: relative;
    display: inline-block;
    margin: 0 15px;
    color: #fff;
    text-decoration: none;
}
header.sticky ul li a{
color: #111;
}

.cta-btn {
    position: relative;
    background: var(--primary-color);
    display: inline-block;
    color: #fff;
    padding: 10px 30px;
    font-size: 16px;
    text-transform: uppercase;
    text-decoration: none;
    letter-spacing: 2px;
    font-weight: 500;
    cursor: pointer;
    left: 100px;
}
.cta-btn:hover {
    color: var(--secondary-color);
}
</style>

