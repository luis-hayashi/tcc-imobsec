<template>
    <header>
            <nav class="navbar">
                <a href="#" class="nav-branding"><img src="../images/logo azul.png" class="img"/></a>
                <ul v-if="hamburguerActive" class="nav-menu active">
                    <li class="nav-item">
                        <a href="/" class="nav-link">Home</a>
                    </li>
                    <li class="nav-item">
                        <a href="/anunciar" class="nav-link">Anunciar</a>
                    </li>
                    <li class="nav-item">
                        <a href="/ofertas" class="nav-link">Ofertas</a>
                    </li>
                    <li class="nav-item">
                        <a href="/simulacao" class="nav-link">Simular</a>
                    </li>
                    <li class="nav-item">
                        <a href="/ajuda" class="nav-link">Ajuda</a>
                    </li>
                    <li class="nav-item">
                        <a href="/sobre" class="nav-link">Sobre</a>
                    </li>
                    <li class="nav-item">
                        <a href="/auth/login" class="nav-link">Entrar</a>
                    </li>
                </ul>
                <ul v-if="hamburguerDesactive" class="nav-menu">
                    <li class="nav-item">
                        <a href="/" class="nav-link">Home</a>
                    </li>
                    <li class="nav-item">
                        <a href="/anunciar" class="nav-link">Anunciar</a>
                    </li>
                    <li class="nav-item">
                        <a href="/ofertas" class="nav-link">Ofertas</a>
                    </li>
                    <li class="nav-item">
                        <a href="/simulacao" class="nav-link">Simular</a>
                    </li>
                    <li class="nav-item">
                        <a href="/ajuda" class="nav-link">Ajuda</a>
                    </li>
                    <li class="nav-item">
                        <a href="/sobre" class="nav-link">Sobre</a>
                    </li>
                    <li class="nav-item">
                        <NuxtLink to="/auth/login" v-if="!user" class="nav-link"> <a> Entrar </a> </NuxtLink>
                        <NuxtLink to="/profile" v-else> <a> Perfil </a> </NuxtLink>
                    </li>
                    <li class="nav-item">
                        <NuxtLink to="/auth/login" v-if="!user" class="nav-link"> <a> Entrar </a> </NuxtLink>
                        <NuxtLink to="/profile" v-else> <a> Perfil </a> </NuxtLink>
                    </li>
                </ul>
                <div v-on:click="toogleBurguerMenu()" v-if="hamburguerDesactive" class="hamburguer">
                    <span v-if="hamburguerDesactive" class="bar"></span>
                    <span v-if="hamburguerDesactive" class="bar"></span>
                    <span v-if="hamburguerDesactive" class="bar"></span>
                </div>
                <div v-on:click="toogleBurguerMenu()" v-if="hamburguerActive" class="hamburguer active">
                    <span v-if="hamburguerActive" class="bar active"></span>
                    <span v-if="hamburguerActive" class="bar active"></span>
                    <span v-if="hamburguerActive" class="bar active"></span>
                </div>
                
        </nav>
    </header>
</template>

<style scoped>
    @import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

* {
    padding: 0;
    margin: 0;
}

header {
    background-color: white;
}

li{
    list-style: none;
}

a{
    color: black;
    text-decoration: none;
    cursor: pointer;
}

.navbar{
    min-height: 70px;
    max-width: 100vw;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 24px;
}

.nav-menu{
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 60px;
}

.nav-link{
    transition: 0.7s ease;
}

.nav-link:hover{
    color: blue;
}

.hamburguer{
    display: none;
    cursor: pointer;
}

.hamburguer span {
    display: block;
    width: 25px;
    height: 3px;
    background-color: #000;
    margin: 5px auto;
    -webkit-transition: all 0.3s ease-in-out;
    transition: all 0.3s ease-in-out;

} 

.img {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100px;
}

@media(max-width:768px){

    .nav-branding img {
        width: 90%;
        height: 90%;
    }
    .navbar {
        padding: 0;
    }

     .hamburguer{
        display: block;
        color: black;
     }

     .hamburguer.active .bar:nth-child(2){
        opacity: 0;
     }

     .hamburguer.active .bar:nth-child(1){
        transform: translateY(8px) rotate(45deg);
     }

     .hamburguer.active .bar:nth-child(3){
        transform: translateY(-8px) rotate(-45deg);
     }

     .nav-menu{
        position: fixed;
        left: -100%;
        top: 90px;
        gap: 0;
        flex-direction: column;
        background-color: #262626;
        width: 100vw;
        text-align: center;
        transition: 0.3s;
     }

     .nav-item{
        margin: 16px 0;
     }

     .nav-item a {
        color: #fff;
     }
     
     .nav-menu.active{
        left: 0;
     }
}
</style>

<script setup>
    const hamburguerActive = ref(false);
    const hamburguerDesactive = ref(true);
    const user = useSupabaseUser();
    const client = useSupabaseClient();

    function toogleBurguerMenu() {
        hamburguerActive.value = !hamburguerActive.value
        hamburguerDesactive.value = !hamburguerDesactive.value
    }
</script>