<template>
    <header>
        <nav>
            <a href="/" class="container"><img src="../assets/logo.png" alt="logo" id="logo"></a>
            <img src="../assets/menu.png" alt="menu-button" id="menu-button" class="container">
            <div id="menu-overlay"></div>
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
}

</style>