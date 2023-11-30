<template>
    <body class="bodiis"></body>
        <navbar/>
        <main>
            <div class="apresentation">
                <div class="text-cont">
                    <h1> Sobre o iMobSec! </h1>
                    <h1> Saiba mais sobre os <br> fundadores e idealização <br> do projeto iMobSec!  </h1>
                    <h1> Confira: </h1>
                    <div class="butt">
                        <a class="btnn" href="/sobre">Sobre nós</a>
                    </div>
                </div>
                <div class="image">
                    <img src="../images/backgg.svg">
                </div>
            </div>

            <div class="dropdown-menu">
            <ul class="ul-dropdown">
                <li class="li-dropdown">
                    <a class="a-dropdown">Cidade ▾</a>
                    <ul class="dropdown">
                        <li><a href="#" class="a-dropdown">São José dos Campos</a></li>
                        <li><a href="#" class="a-dropdown">Rio de Janeiro</a></li>
                        <li><a href="#" class="a-dropdown">Belo Horizonte</a></li>
                    </ul>
                </li>                           
            </ul>
            <ul class="ul-dropdown">
                <li class="li-dropdown">
                    <a class="a-dropdown">Estado ▾</a>
                    <ul class="dropdown">
                        <li><a href="/search/sp" class="a-dropdown">São Paulo</a></li>
                        <li><a href="#" class="a-dropdown">Rio de Janeiro</a></li>
                        <li><a href="#" class="a-dropdown">Minas Gerais</a></li>
                    </ul>
                </li>                           
            </ul>

            <div class="SearchBar">
                <table class="elementsSearch">
                    <tr>
                        <td>
                            <input type="text" placeholder="Buscar..." class="search">
                        </td>
                    </tr>
                </table>
            </div>

            <ul class="ul-dropdown">
                <li class="li-dropdown">
                    <a class="a-dropdown">Filtros ▾</a>
                    <ul class="dropdown">
                        <li><a href="#" class="a-dropdown">Casa</a></li>
                        <li><a href="#" class="a-dropdown">Apartamento</a></li>
                        <li><a href="#" class="a-dropdown">Condomínio</a></li>
                    </ul>
                </li>                           
            </ul>

            <div class="container-btn">
                <button type="submit" class="btn-buscar">Buscar</button>
            </div>
        </div>

        <h1>Anúncios em destaque perto de você</h1>

        <div class="ad-card">
<div class="anuncio-wrapper">

    <div class="ad-photo">
        <img src="../images/casa1.jpg" style="color: #bcbcbc;" />
    </div>
    <div class="ad-content">
        <div class="ad-content-left">
            <div class="ad-content-left-top">
                <a href="/id/ajuissjiujdHHFS1">Casa no Urbanova em bom estado</a>
                <p>Urbanova, São José dos Campos</p>
            </div>
            <div class="ad-content-left-middle">
                Casa bem acomodada com quatro quartos e três banheiros.
            </div>
            <div class="ad-content-left-bottom">
                <img src="../images/vector.svg" alt="heart" class="imgad">
            </div>
        </div>
        <div class="ad-content-right">
            <h4>R$ 654.000</h4>
            <p>R$ 196.200</p>
        </div>
    </div>
</div>
</div>

        <div class="ad-card">
            <div class="anuncio-wrapper">

                <div class="ad-photo">
                    <img src="../images/casa2.jpg" style="color: #bcbcbc;" />
                </div>
                <div class="ad-content">
                    <div class="ad-content-left">
                        <div class="ad-content-left-top">
                            <a href="/id/ajdifjJklaASd92">CASA EM CONDOMINIO FECHADO PARA ALUGAR!</a>
                            <p>Barra da Tijuca, Rio de Janeiro</p>
                        </div>
                        <div class="ad-content-left-middle">
                            Casa em condominio fechado com segurança 24h.
                        </div>
                        <div class="ad-content-left-bottom">
                            <img src="../images/vector.svg" alt="heart" class="imgad">
                        </div>
                    </div>
                    <div class="ad-content-right">
                        <h4>R$ 750/dia</h4>
                        <p>ALUGAR</p>
                    </div>
                </div>
            </div>
        </div>

        <div class="ad-card">
            <div class="anuncio-wrapper">

                <div class="ad-photo">
                    <img src="../images/casa3.jpg" style="color: #bcbcbc;" />
                </div>
                <div class="ad-content">
                    <div class="ad-content-left">
                        <div class="ad-content-left-top">
                            <a href="/id/hrrfpAhHG102">Sítio para temporada na Pampulha</a>
                            <p>Pampulha, Belo Horizonte</p>
                        </div>
                        <div class="ad-content-left-middle">
                            Sítio para temporada na Pampulha com piscina
                        </div>
                        <div class="ad-content-left-bottom">
                            <img src="../images/vector.svg" alt="heart" class="imgad">
                        </div>
                    </div>
                    <div class="ad-content-right">
                        <h4>R$ 1.027/dia</h4>
                        <p>TEMPORADA</p>
                    </div>
                </div>
            </div>
        </div>
        
        <footerComp/>
        </main>
</template>

<script setup>

</script>

<style scoped>
    @import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

    * {
       font-family: 'Poppins', sans-serif;
    }

    .bodiis {
        margin: 0;
        padding: 0;
    } 

    .imgad {
        cursor: pointer ;
    }

    .apresentation {
        display: flex;
        flex-direction: row;
        margin: 0;
    }

    main {
        padding: 0;
        margin: 0;
    }

    .text-cont {
        display: flex;
        width: 45vw;
        height: 47.2vh;
        gap: 20px;
        flex-direction: column;
        color: white;
        background: #193083;
        justify-content: center;
        padding-left: 20px;
    }
    
    .butt {
        display: flex;
        justify-content: center;
    }

    h1 {
        font-size: 1.8rem;
        font-weight: 400;
    }

    .btnn {
        display: flex;
        align-items: center;
        justify-content: center;
        background: #fff;
        color: #193083;
        border: none;
        border-radius: 8px;
        width: 180px;
        font-size: 1.4rem;
        height: 50px;
        cursor: pointer;
        text-decoration: none;
        transition: .2s;
    }

    .btnn:active {
        padding: 20px;
        transition: .2s;
    }
    .dropdown-menu {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 10rem;
}

.ul-dropdown {
    list-style: none;
    background: white;
}

.ul-dropdown .li-dropdown {
    display: inline-block;
}

.ul-dropdown .li-dropdown .a-dropdown {
    display: flex;
    padding: 1rem 0.8rem;
    color: rgba(35, 33, 33, 0.500);
    text-decoration: none;
    text-align: center;
    font-size: 17px;
    background-color: #ededed;
    border-radius: 10px;
    transition: 0.3s;
}

.ul-dropdown .li-dropdown ul.dropdown {
    width: 100%;
    background: #ededed;
    position: absolute;
    z-index: 999;
    display: none;
    overflow-y: auto;
    width: 180px;
    height: 100px;
}

.ul-dropdown .li-dropdown a:hover {
    background: #0e1e56;
    color: white;
}

.ul-dropdown .li-dropdown:hover ul.dropdown {
    display: block;
}

.SearchBar {
    position: flex;
    width: 500px;
    height: 50px;
    background-color: #ededed;
    padding: 0px 10px;
    border-radius: 10px;
}

.elementsSearch {
    width: 100%;
    height: 100%;
}

.search {
    border: none;
    height: 100%;
    width: 100%;
    padding: 0px 5px;
    border-radius: 10px;
    text-decoration: none;
    outline: none;
    background-color: #ededed;
    font-size: 17px;
}

.search:focus {
    outline: none;
}

.btn-buscar {
    width: 80px;
    height: 45px;
    background-color: #193083;
    color: white;
    font-size: 15px;
    border-radius: 10px;
    border: none;
    cursor: pointer;
}

    .ad-card {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    background-color: white;
    margin-top: 1rem;
    margin-bottom: 2rem;
}

.anuncio-wrapper {
    display: flex;
    background-color: #ededed;
    width: 70%;
    height: 200px;
    border-radius: 1.2rem;
    box-shadow: 2px 4px 3px 2px rgba(0, 0, 0, 0.400);
    padding: 0.7rem;
}

.ad-photo {
    height: 100%;
    padding: 0 4rem;
    display: flex;
    align-items: center;
    justify-content: center;
    border-right: 1px solid #bcbcbc;
}

.ad-photo img {
    width: 200px;
}

.ad-content {
    padding: 0 1rem;
    padding-left: 1.5rem;
    display: flex;
    justify-content: space-between;
    width: 100%;
}

.ad-content-left-top a {
    font-weight: 400;
    font-size: 0 1rem;
    cursor: pointer;
}

.ad-content-left-top p {
    font-weight: 400;
    font-size: 0.9rem;
    margin-left: 3px;
}

.ad-content-left {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}

.ad-content-right {
    width: 10vw;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
}

.ad-content-right h4 {
    display: flex;
    justify-content: center;
    font-weight: 500;
    color: #193083;
    font-size: 1.2rem;
}

.ad-content-right p {
    display: flex;
    justify-content: center;
    font-weight: 400;
    font-size: 0.92rem;
}

.ad-content-left-bottom img {
    width: 25px;
    margin: 10px;
}

</style>