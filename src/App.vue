<template>
  <Header />
  <Banner />
  <Subscribe />
  <Blogs />

</template>

<script>
import Header from './components/Header.vue'
import Banner from './components/Banner.vue'
import Subscribe from './components/Subscribe.vue'
import Blogs from './components/Blogs.vue'



export default {
  name: 'App',
  components: {
    Header,
    Banner,
    Subscribe,
    Blogs,
  }
}
</script>

<style>
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    scroll-behavior: smooth;
    --primary-color:#628d49;
    --secondary-color:#ffbd6e;


}

#app {
  /* font-family: Avenir, Helvetica, Arial, sans-serif; */
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

h1, h2, h3, h4, h5, h6, a, button{
    font-family: "Press Start 2P"
}

section{
    padding: 100px;
}

@media (max-width: 991px){
    header,
    header.sticky{
        padding: 20px 50px;
        z-index: 1000;
    }
    .menu{
        position: fixed;
        top: 75px;
        left: -100%;
        display: block;
        padding: 100;
        text-align: center;
        width: 100%;
        height: 100vh;
        background: white;
        transition: 0.5s;
        z-index: 999;
        border-top: 1px solid rgba(0,0,0,0.2);
    }
    .menu.active{
        left: 0;
    }
    header ul li a{
        color: #111;
        font-size: 24px;
        margin: 10px;

    }
    .toggle{
        width: 40px;
        height: 40px;
        background: url(./assets/menu.png);
        background-position: center;
        background-repeat: no-repeat;
        background-size: 30px;
        cursor: pointer;
    }
    .toggle.active{
        width: 40px;
        height: 40px;
        background: url(./assets/close.png);
        background-position: center;
        background-repeat: no-repeat;
        background-size: 25px;
        cursor: pointer;

    }
    header .toggle{
        filter: invert(1)
    }
    header.sticky .toggle{
        filter: invert(0)
    }
    section{
        padding: 100px 50px;
    }
    .banner{
        padding: 150px 50px 100px;
    }
    .btn{
        margin: 10px;
        padding: 10px 20px;
        font-size: 16px;
    }
    .heading h2{
        font-weight: 600;
        font-size: 24px;
    }
    .contentBox h3{
        font-size: 20px;
    }
    .content{
        flex-direction: column;
    }
    .w50{
        margin-bottom: 20px;
    }
    .services .content .servicesBox{
        margin: 10px;
    }
    .project .content {
        align-items: center;
    }

    .project .content .projectBox {
        padding: 10px;
    }
    .contact .content {
        flex-direction: row;
    }
    /* .testimonials .content .testimonialsBox {
        max-width: calc(100% - 20px);
        padding: 40px 20px;
        margin: 10px;
        background: rgb(244,198, 137);
    }
        .testimonials .content .testimonialsBox h3 {
            margin-top: 20px;
    } */
    .contactInfo {
        margin: 20px 0;
    }
}

@media (max-width:600px){
    header,
    header.sticky{
        padding: 20px 20px;
        z-index: 1000;
    }
    .banner{
        padding: 150px 20px 100px;
    }
    section{
        padding: 100px 20px;
    }
    .banner h2{
        font-size: 2.5em;
    }
    .banner h3{
        font-size: 1em;
    }
}
</style>
