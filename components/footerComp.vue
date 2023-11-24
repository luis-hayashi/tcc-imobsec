<template>
    <body class="bodie">
    <footer>
        <div class='footer-section'>
            <div class='logo'>
                <img src = "../images/icone branco.png" alt="logo-icon" class='logo-icon'/>
            </div>

            <div class='Section'>
            <h1>O iMobSec</h1>
            <p>O iMobSec é um projeto que ajuda os usuários a encontrar imóveis online de forma segura e prática, com recursos de privacidade, navegação eficiente e é um parceiro valioso para profissionais imobiliários.</p>
            </div>

            <div class='Section'>
                <h1>Atalhos</h1>
                        
                        <a href="/home" class='link-atalhos'>Home</a>
                        

                        <a href="/Anunciar" class='link-atalhos'>
                            anunciar
                        </a>

                        <a href="/Ofertas" class='link-atalhos'>
                            Ofertas
                        </a>

                        <a href="/Simular" class='link-atalhos'>
                            Simular
                        </a>

                        <a href="/ajuda" class='link-atalhos'>
                            Ajudar
                        </a>

                        <a href="/Sobre_nós" class='link-atalhos'>
                            Sobre
                        </a>

                        <a href="/Login" class='link-atalhos'>
                            Perfil
                        </a>
            </div>

            <div class='Section'>
                <h1>Ajuda</h1>
                    <a href="" class='link-ajuda'>
                    mobsecp@gmail.com
                    </a>

                    <a href="" class='link-ajuda'>
                        +55 (12)99651-5989
                    </a>

                    <a href="" class='link-ajuda'>
                        Chat Suporte
                    </a>

                    <a href="" class='link-ajuda'>
                        FAQ
                    </a>
            </div>

            <div class='Section'>
                
                <h1>Mídias Sociais</h1>
                    <a href="" class='Social-Media-link'>
                        <img src="../images/facebookic.png"/>
                    </a>

                    <a href="" class='Social-Media-link'>
                        <img src="../images/instagramic.png">
                    </a>

                    <a href="" class='Social-Media-link'>
                        <img src="../images/linkedinic.png">
                    </a>
            </div>
        </div>
        <div class='copyright'>
            <p>Copyright ©  2023, iMobSec. All Rights Reserved </p>
        </div>
    </footer>
</body>
</template>

<style scoped>

footer img {
    width: 50px;
    height: 50px;
}

* {
    margin: 0;
    padding: 0;
}

.bodie {
    margin: 0;
}

.footer-section{
    display: flex;
    width: 100%;
    margin: 0;
    gap: 10px;
    padding-top: 10px;
    padding-bottom: 10px;
    justify-content: center;
    align-items: center;
    background: #193083;
}

.copyright{
    display: flex;
    padding: 5px;
    justify-content: center;
    background-color: #0e1e56;
}

.copyright p{
    font-size: 12px;
    color: #ffffff;
}

.logo{
    display: flex;
    height: 100;  
    align-items: center;
}

.Section{
    display: flex;
    flex-direction: column;
    width: 22%;
    padding: 0 15px;
}

.Section h1{
    font-size: 18px;
    color: #ffff;
    text-transform: capitalize;
    margin-bottom: 30px;
    font-weight: 500;
    position: relative;
}

.Section h1::before{
    content: '';
    position: absolute;
    left: 0;
    bottom: -10px;
    background-color: #ffffff;
    height: 2px;
    box-sizing: border-box;
    width: 50px;
}

.Section a{
    font-size: 15px;
    text-transform: capitalize;
    color: #ffffff;
    text-decoration: dotted;
    font-weight: 300;
    color: #ffffff;
    display: block;
    transition: all 0.3s ease;
}

a:hover{
    padding-left: 8px;
    color: #ffffff;
}

.Section p{
    font-size: 15px;
    text-transform: capitalize;
    color: #ffffff;
    text-decoration: dotted;
    font-weight: 300;
    color: #ffffff;
    display: block;
}

.Section img{
    align-items: center;
}


.Social-Media-link img{
    flex-direction: row;
    display: inline-block;
    height: 40px;
    width: 40px;
    margin: 0 10px 10px 0;
    text-align: center;
    line-height: 40px;
    transition: all 0.5s ease;
}

/*Responsivo*/

@media (max-width: 574px){
    .footer-section{
        flex-direction: column;
        gap: 15px 0;
    }

    .Section {
        width: 100vw;
        align-items: center;
    }
}
</style>