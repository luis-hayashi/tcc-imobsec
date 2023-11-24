<template>
    <body class="bori">
        <div class="backgroundd">
        </div>
        <div class="bg">
                <div class="card">
                    <div class="cardazul">
                        <div class="logo">
                        <img src='../../images/logo branca.png' alt="" />
                        </div>
                            <div class="white-text">
                            <p class="titulo"> Bem-Vindo ao iMobSec!</p>
                            <p class="texto-descritivo">Faça o seu login e acesse sua conta agora mesmo!</p>
                        </div>
                        <div class="button">
                            <a href="/auth/login" class="entrar">ENTRAR</a>
                        </div>
                    </div>
                    <div class="cardbranco">
                        <div class="blue-text">
                            <p class="crie">Crie sua conta!</p>
                            <p class="linkempresarial">criando uma conta pessoal? <a href="/auth/register">clique aqui!</a></p>
                        </div>
                        <form action="../auth/sign-up-emp"
                        method="post">
                            <div class="msgg">
                                <Messages/>
                            </div>
                            <div class="textboxs"> 
                                <input type="text" placeholder="Usuário" class="box" name="username" />
                                <input type="text" placeholder="E-mail" class="box" name="email" required/>
                                <input type="password" placeholder="Senha" class="box" name="password" required/>
                                <input type="number" placeholder="CNPJ" class="box" name="cnpj" />
                            </div>
                            <div class="button">
                                <button class="cadastrar"> CADASTRAR</button>
                            </div>
                        </form>
                    </div>
                </div>
            </div>
    </body>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

.backgroundd {
    background-image: url("../../images/background.png");
    background-size: 100vw 100vh;
    z-index: -1;
    position: fixed;
    width: 100vw;
    height: 100vh;
    background-repeat: no-repeat;
}

* {
    font-family: 'Poppins', sans-serif;
    padding: 0;
    margin: 0;
    box-sizing: content-box;
}

body {
    padding: 0;
    margin: 0;
    overflow: hidden;
}

.bg {
    width: 100vw;
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
}

.card{
    width: 80vw;
    height: 80vh;
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
}

.cardazul{
    background-color: #193083;
    min-width: 32%;
    min-height: 100%;
    max-height: 100%;
    justify-content: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    gap: 40px;
    border-radius: 20px 0 0 20px;
    box-shadow: 5px 4px 10px 0px rgba(0, 0, 0, 0.25);
    overflow: hidden;
}

.cardazul img{
    width: 400px;
}

.logo{
    display: flex;
    height: 200px;
    align-items: flex-start;
    justify-content: flex-start;
}

.titulo{
    color: #FFF;
    font-family: Poppins;
    font-size: 24px;
    font-style: normal;
    font-weight: 900;
    line-height: normal;
}

.texto-descritivo{
    color: #FFF;
    font-family: 'Poppins', sans-serif;
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

.cardbranco {
    background-color: #FFFFFF;
    min-width: 70%;
    min-height: 100%;
    max-height: 100%;
    align-items: center;
    justify-content: center;
    display: flex;
    flex-direction: column;
    gap: 10px;
    border-radius: 0 20px 20px 0;
    box-shadow: 5px 4px 10px 0px rgba(0, 0, 0, 0.25);
    overflow: hidden;
}

.crie{
    color: #193083;
    text-align: center;
    font-family: Poppins;
    font-size: 24px;
    font-style: normal;
    font-weight: 900;
    line-height: normal;
}

.linkempresarial{
    color: #193083;
    font-family: Poppins;
    font-size: 14px;
    font-style: normal;
    font-weight: 900;
    line-height: normal;
}

.textboxs{
    align-items: center;
    justify-content: center;
    display: flex;
    flex-direction: column;
    gap: 10px;
}

.box{
    min-width: 35vw;
    min-height: 7vh;
    border-radius: 10px;
    background: #DFDFDF;
    font-weight: 900;   
    outline: none;
    border: none;
    padding: 0 0 0 10px;
    padding-left: 40px;
    font-family: Poppins;
    font-size: 14px;
    font-style: normal;
    font-weight: 900;
    line-height: normal;
}

.object {
    display: flex;
    min-width: 38vw;
}

.box::placeholder{
    color: #BCBCBC;
    font-family: Poppins;
    font-size: 14px;
    font-style: normal;
    font-weight: 900;
    line-height: normal;
}

.radios{
    display: flex;
    justify-content: center;
    gap: 10px;
    min-width: 38vw;
    gap: 8px;
}

.radios label{
    color: rgba(0, 0, 0, 0.80);
    font-family: Poppins;
    font-size: 10px;
    font-style: normal;
    font-weight: 900;
    line-height: normal;
}


.objetive{
    width: 100%;
    display: flex;
    justify-content: center;
    color: #29429A;
    font-family: Poppins;
    font-size: 15px;
    font-style: normal;
    font-weight: 900;
    line-height: normal;
}

.entrar {
    outline: none;
    background: #193083;
    border: solid #fff;
    padding: 10px;
    color: #fff;
    border-radius: 30px;
    padding: 20px;
    padding-left: 50px;
    padding-right: 50px;
    font-weight: 900;
    transition: .2s;
    cursor: pointer;
}

.entrar:hover {
    background: #fff;
    color: #193083;
    transition: .2s;
}

.entrar:active {
    padding: 30px;
    padding-left: 60px;
    padding-right: 60px;
    transition: .1s;
}

.cadastrar {
    display: flex;
    justify-content: center;
    outline: none;
    background: #fff;
    border: solid #193083;
    padding: 10px;
    color: #193083;
    border-radius: 30px;
    padding: 20px;
    padding-left: 50px;
    padding-right: 50px;
    font-weight: 900;
    transition: .2s;
    cursor: pointer;
}

.cadastrar:hover {
    background: #193083;
    color: #fff;
    transition: .2s;
}

.cadastrar:active {
    padding: 30px;
    padding-left: 60px;
    padding-right: 60px;
    transition: .1s;    
}

@media screen and (max-width: 450px) {
    .cardazul {
        display: none;
    }
    
    .cardbranco {
        border-radius: 20px 20px 20px 20px;
        padding: 20px;
    }
}

a {
    text-decoration: none;
    color: #193083;
}

input[type=number]::-webkit-inner-spin-button {
    -webkit-appearance: none;
}

.msgg {
    display: flex;
    justify-content: center;
}

.button {
    display: flex;
    justify-content: center;
    padding-top: 20px;
}
</style>