<template>
  <div>
    <nav>
      <div class="logo">
        <a href="/"><h4>Awapuni</h4><h4> Takeaways</h4></a>
      </div>
      <ul class="nav-links">
        <li><a href="/">Home</a></li>
        <li>|</li>
        <li><a href="#about">About</a></li>
        <li>|</li>
        <li><a href="#menu">Menu</a></li>
        <li>|</li>
        <li><a href="#contact">Contact</a></li>
      </ul>
      <div class="burger">
        <div class="line"></div>
        <div class="line"></div>
        <div class="line"></div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
    name: "Navbar"
};
</script>

<style scoped>

nav {
    display:flex;
    justify-content: space-around;
    align-items: center;
    min-height: 11vh;
    background-color:midnightblue;
    position: fixed;
    width:100vw;
    top: 0;
}

.logo{
    display: flex;
    color:whitesmoke;
    text-transform: uppercase;
    letter-spacing: 7px;
    font-size: 20px;
}

.logo a{
    text-decoration: none;
    color:whitesmoke;
}

.nav-links{
    display: flex;
    justify-content: space-around;
    width: 35%;
    height: 100%;
}
.nav-links li {
    list-style: none;
    text-decoration: none;
    color:whitesmoke;
}

.nav-links a {
    color:whitesmoke;
    text-decoration: none;
    letter-spacing: 3px;
    font-weight: lighter;
    font-size: 15px;
}


.burger{
    display: none;
}

.burger div {
    width:25px;
    height:3px;
    background-color: rgb(226, 226, 226);
    margin: 5px;

}
@media screen and  (max-width: 1024px){
    .nav-links{
        width: 60%;
    }
}

@media screen and  (max-width: 768px){
    body{
        overflow-x: hidden;
    }
    .nav-links{
        display: flex;
        flex-direction: column;
        align-items: center;
        position: absolute;
        right: 0px;
        height: 92vh;
        top: 8vh;
        background-color: grey;
        width: 100%;
        transform: translateX(100%); 
        clip-path: circle(100px at 90% -10%);
        -webkit-clip-path: circle(100px at 90% -10%);
        transition: all 1s ease-out;
        /* transition: transform 0.5s ease-in;  */
    }
    .nav-links li{
        opacity: 0;
    }
    .burger {
        display: block;
        cursor: pointer;
    }
}

.nav-active{
    transform: translateX(0%);
    clip-path: circle(1000px at 90% -10%);
    -webkit-clip-path: circle(1000px at 90% -10%);
}
</style>
