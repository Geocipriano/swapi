<template>
    <header>
        <nav>
            <a href="/" class="container"><img src="../assets/logo.png" alt="logo" id="logo"></a>
            <img src="../assets/menu.png" alt="menu-button" id="menu-button" class="container">
            <div id="menu-overlay" v-if="menuActive"></div>
            <div id="menu-itens" :class="{active:menuActive}">
                <a href="/"><img src="../assets/logo.png" alt="logo" id="menu-logo"></a>
                <ul>
                    <li><a href="/">Home</a></li>
                    <li><a href="/sobre">Sobre</a></li>
                    <li><a href="/filmes">Filmes</a></li>
                </ul>
            </div>
        </nav>
    </header>
</template>

<script>
export default {
    name: 'Navbar',
    data(){
        return{
            menuActive: true
        }
    }
}
</script>

<style scoped>
header {
    background-color: var(--color-black);
    height: 60px;
    width: 100%;
}
nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
}
#logo {
    width: 70px;
}
#menu-button {
    width: 70px;
    color: white;
}
#menu-overlay {
    position: fixed;
    top: 0;
    left: 0;
    width: 40%;
    height: 100vh;
    background-color: #0000;
    opacity: 0.8;
}
#menu-logo {
    width: 110px;
}
#menu-itens {
    position: fixed;
    top: 0;
    right: 0;
    background-color: var(--color-black);
    width: 60%;
    height: 100vh;
    display: none;
    flex-direction: column;
    justify-content: flex-start;
    align-items: center;
}
#menu-itens .active {
    display: flex;
}
#menu-itens ul li {
    margin-bottom: 20px;
}

#menu-itens ul {
    text-align: center;
}

#menu-itens ul li a {
    font-size: 20px;
    color: var(--color-yellow);
}
</style>