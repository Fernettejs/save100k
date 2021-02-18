<template>
    <section class="project" id="project">
    <div class="heading">
        <h2>My Latest Blogs</h2>
    </div>
    <div class="content">
        <div class="projectBox">
            <a href="http://backfirstresponders.github.io/" target="_blank">
                <img src="../assets/safe.png.jpg" alt="">
                <div class="projectText"><b>Alex's Portfolio:</b> <br/><br/> Personal website for my wife using HTML, CSS, and minimal JS.</div>
            </a>
        </div>
        <div class="projectBox">
            <a href="Week1" target="_blank">
                <img src="../assets/safe.png.jpg" alt=""> 
                <div class="projectText"><b>JavaScript Car Game</b> <br/><br/> Simple game with primary focus on JavaScript (so don't hate on the lack of design).</div>
            </a>
        </div>
    </div>
</section>
</template>

<style scoped>
.project{
    background: var(--light-color);
}
.project .content {
    display: flex;
    justify-content: space-evenly;
    flex-wrap: wrap;
}
.project .content .projectBox {
    width: 350px;
    height: 350px;
    padding: 20px;
    position: relative;
    text-align: center;
}
.project .content .projectBox img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    background: rgba(24, 39, 54, 0.65);
    opacity: 1;
    display: block;
    transition: .5s ease;
    backface-visibility: hidden;
    background-color: white;
    box-shadow: 3px 6px rgba(0, 0, 0, 0.25);
    border-radius: 10px;
    z-index: 99;

}
.projectText{
    transition: .5s ease;
    transform: translate(-50%, -50%);
    text-align: center;
    background: #85bb65;
    color: #fff;
    visibility: hidden;
    opacity: 0;
    padding: 32px 64px;
    height: 300px;
    width: 300px;
    position: absolute;
    top: 50%;
    left: 50%;
}
.projectBox:hover .projectText{
    visibility: visible;
    opacity: 1;
    border-radius: 10px;
}
.projectBox:hover img{
    filter: opacity(.3);
}

</style>


<script>
export default {
    
}
</script>