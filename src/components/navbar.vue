<template>
    <header>
        <nav>
            <a href="/"><img src="../assets/logo.png" alt="logo" id="logo"></a>
            <img src="../assets/menu.png" alt="menu-button" id="menu-button">
        </nav>
    </header>
</template>

<script>
export default {
    name: 'Navbar'
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
    
}
#logo {
    width: 70px;
}
#menu-button {
    width: 40px;
    color: white;
}
</style>