<template>
    <body>
        
    </body>
    <main>
        <navbar/>
        <div class="layout">
            <div class="background-case">
                
            </div>

            <div class="top-row">
                <div class="left-col">
                    <div class="photo">
                        <img src="../images/eu.png" alt="foto-perfil">
                    </div>

                    <div class="profile-content">
                        <div class="line-1">
                            <h1 class="name">Luis Felipe</h1>
                            <div class="verify">
                                <i class="fa-solid fa-check-circle" style="color: #193083;"></i>
                                <p> Em atividade desde 2023</p>
                            </div>
                        </div>

                        <div class="status">
                            <i class="fa-solid fa-circle fa-xs" style="color: rgb(48, 241, 0);"></i>
                            <p>Online</p>
                        </div>

                        <div class="info">
                            <p class="descri">São José dos Campos, SP.</p>
                            <p class="descri"></p>
                        </div>
                    </div>
                </div>


                <div class="right-col">
                    <img class="wplogo" src="../images/wplogo.png">
                    <button class="message-button">
                        +55 (12) 98154-7200</button>
                </div>
            </div>
        </div>

        <div class="main-col">
            <div class="mid-row">
                <div class="left-buttons">
                    <h1>Anúncios</h1>
                </div>

                <div class="right-select">
                    <input type="radio" name="tipo-imovel" id="Destaque">
                    <label for="Destaque">Destaques</label>

                    <input type="radio" name="tipo-imovel" id="Todos">
                    <label for="Todos">Todos</label>

                    <input type="radio" name="tipo-imovel" id="Temporada">
                    <label for="Temporada">Temporada</label>

                    <input type="radio" name="tipo-imovel" id="Comprar/Alugar">
                    <label for="Comprar/Alugar">Comprar/Alugar</label>
                </div>
            </div>

            <div class="ad-card">
            <div class="anuncio-wrapper">

                <div class="ad-photo">
                    <img src="../images/casa1.jpg" style="color: #bcbcbc;" />
                </div>
                <div class="ad-content">
                    <div class="ad-content-left">
                        <div class="ad-content-left-top">
                            <a>Casa no Urbanova em bom estado</a>
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
                        <p>R$ 200.000</p>
                    </div>
                </div>
            </div>
        </div>
        </div>
        <footerComp/>
    </main>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

* {
    margin: 0;
    padding: 0;
    font-family: "Poppins", sans-serif;
}

.layout {
    margin: 0;
}

body {
    margin: 0;
    padding: 0;
}

.background-case {
    display: flex;
    flex-direction: row;
    background-color: #bdbcbc;
    width: 100%;
    height: 45vh;
    align-items: center;
    justify-content: center;
    margin: 0;
}

.wplogo {
    width: 100px;
}

.background-case img {
    height: 15vh;
}

.top-row {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    margin: 10px;
    margin-bottom: 20PX;
}

.left-col {
    display: flex;
    flex-direction: row;
    margin-top: 10px;
}

.photo {
    display: flex;
    flex-direction: column;
    justify-content: left;
    align-items: center;
    gap: 5px;
}

.photo img {
    height: 120px;
}

.profile-content {
    display: flex;
    flex-direction: column;
    margin-left: 20px;
}

.line-1 {
    display: flex;
    flex-direction: row;
    gap: 8px;
    margin: 0px;
}

.name {
    margin: 0;
    font-size: 30px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    margin-right: 5px;
}

.verify {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    gap: 5px;
}

.verify p {
    margin: 0;
    color: rgba(0, 0, 0, 0.45);
    font-weight: 400;
    font-size: 15px;
}

.status {
    display: flex;
    flex-direction: row;
    align-items: center;
    gap: 5px;
    margin-top: 10px;
    margin-bottom: 10px;
}

.status p {
    font-size: 13px;
    margin: 0;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

.info {
    display: flex;
    flex-direction: column;
}

.info p {
    margin: 3px;
    font-size: 14px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

.right-col {
    display: flex;
    flex-direction: row;
    gap: 20px;
    margin-top: 10px;
    align-items: center;
}

.message-button {
    background-color: white;
    border: 3px solid rgba(0, 0, 0, 0.60);
    border-radius: 10px;
    color: rgba(0, 0, 0, 0.60);
    font-size: 18px;
    text-align: center;
    align-items: center;
    justify-content: center;
    height: 8vh;
    width: 16vw;
}

.message-button:hover {
    background-color: #193083;
    color: white;
    border: none;
    transition: 0.8s all ease;
}

.message-button:active {
    transform: scale(1);
    background-position: 500px;
    padding: 20px;
    transition: .2s;
}

.social-media {
    display: flex;
    flex-direction: row;
    gap: 20px;
    align-items: center;
    margin-top: 20px;
}

.mid-row {
    margin: 15px;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
}

.left-buttons {
    display: flex;
    flex-direction: row;
    align-items: center;
    gap: 12px;
}

.left-buttons h1 {
    font-size: 22px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

.filter {
    align-items: center;
    background-color: #EDEDED;
    color: #7F7F7F;
    border: none;
    border-radius: 10px;
    font-size: 15px;
    height: 8vh;
    width: 8vw;
}

.filter img {
    height: 2.5vh;
}

.right-select {
    margin: 15px;
}

.right-select input[type="radio"] {
    opacity: 0;
    position: fixed;
    width: 0;
}

.right-select label {
    display: inline-block;
    padding: 10px 20px;
    font-family: sans-serif, Arial;
    font-size: 16px;
    transition: 0.2s;
}

.right-select label:hover {
    border-bottom: 4px solid #19308377;
    transition: 0.2s;

}

.right-select input[type="radio"]:checked+label {
    border-bottom: 4px solid #193083;
}

.ad-card {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    background-color: white;
    margin-top: 20px;
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

.ad-content-left-top h2 {
    font-weight: 400;
    font-size: 0 1rem;
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