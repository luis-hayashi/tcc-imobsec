<template>
    <body>
    </body>
    <navbar/>
    <main>
        <div class="top-row">
            <div class="photos">
                <div class="main-photo">
                    <img src="../../images/casa3.jpg" alt="#">
                </div>
            </div>

            <div class="right-content">
                <div class="ad-title">
                    <h1 class="titulo"> Sítio para temporada na Pampulha </h1>
                    <p class="data-post"> Publicado em 20 de Novembro de 2023 </p>
                    <p class="ad-code"> cód. 000000002 </p>
                </div>

                <div class="price">
                    <h1 class="valor">R$ 1.027/dia</h1>
                    <p class="entrada"> TEMPORADA</p>
                    <a class="contact" href="/contact/contact3"><i class="fa-solid fa-message fa-sm"></i>CONTATAR</a>
                </div>
            </div>
        </div>

        <div class="info">
            <div class="descrip">
                <h1 class="info-sec">Descrição</h1>
                <p class="descrip-sec">Sítio para temporada na Pampulha com piscina
                </p>
            </div>

            <div class="rooms">
                <h1 class="info-sec">Principais características</h1>

                <div class="rooms-icons">
                    <div class="room-info">
                        <i class="fa-solid fa-bed fa-xk"></i>
                        <p>6 dormitórios</p>
                    </div>
                    <div class="room-info">
                        <i class="fa-solid fa-toilet-paper fa-xl"></i>
                        <p>4 banheiros</p>
                    </div>
                    <div class="room-info">
                        <i class="fa-solid fa-stairs fa-xl"></i>
                        <p>2 andares</p>
                    </div>
                    <div class="room-info">
                        <i class="fa-solid fa-car fa-xl"></i>
                        <p>5 vagas</p>
                    </div>
                    <div class="room-info">
                        <i class="fa-solid fa-ruler fa-xl"></i>
                        <p>123m²</p>
                    </div>
                </div>
            </div>

            <div class="add-rooms">
                <h1 class="info-sec">Adicionais do imóvel</h1>
                <div class="additional">
                    <div class="col-1">
                        <div class="checkbox">
                            <label for="Piscina">Piscina</label>
                        </div>
                        <div class="checkbox">
                            <label for="Sauna">Sauna</label>
                        </div>
                        <div class="checkbox">
                            <label for="Academia">Academia</label>
                        </div>
                        <div class="checkbox">
                            <label for="Quadra">Quadra</label>
                        </div>
                        <div class="checkbox">
                            <label for="Espaçopet">Espaço pet</label>
                        </div>
                    </div>
                    <div class="col-2">
                        <div class="checkbox">
                            <label for="gourmet">Espaço gourmet</label>
                        </div>
                        <div class="checkbox">
                            <label for="pizza">Forno para pizza</label>
                        </div>
                        <div class="checkbox">
                            <label for="Churrasqueira">Churrasqueira</label>
                        </div>
                        <div class="checkbox">
                            <label for="Horta">Horta</label>
                        </div>
                        <div class="checkbox">
                            <label for="festas">Salão de festas</label>
                        </div>
                    </div>
                    <div class="col-3">
                        <div class="checkbox">
                            <label for="Brinquedoteca">Brinquedoteca</label>
                        </div>
                        <div class="checkbox">
                            <label for="Playground">Playground</label>
                        </div>
                        <div class="checkbox">
                            <label for="leitura">Espaço para leitura</label>
                        </div>
                        <div class="checkbox">
                            <label for="Cinema">Cinema pessoal</label>
                        </div>
                        <div class="checkbox">
                            <label for="jogos">Salão de jogos</label>
                        </div>
                    </div>
                </div>
            </div>

            <div class="map-sec">
                <div class="local">
                    <h1 class="info-sec">Localização</h1>
                    <p class="local-descrip">R. Mascarenhas de Morais, Pampulha - Belo Horionte, MG
                    </p>
                    <p class="cep">CEP: 31270-720</p>
                </div>
            </div>
        </div>
        <footerComp/>
    </main>
</template>

<style scoped>
    @import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

* {
    font-family: "Poppins", sans-serif;
    margin: 0;
    padding: 0px;
}

.layout {
    padding: 15px;
}

.top-row {
    display: flex;
    flex-direction: row;
}

.map-sec {
    margin-bottom: 50px;
}

.photos {
    display: flex;
    flex-direction: column;
}

.main-photo {
    display: flex;
    background-color: #BCBCBC;
    width: 53vw;
    height: 63vh;
    justify-content: center;
    border-radius: 15px;
}

.selec-photos {
    display: flex;
    flex-direction: row;
    gap: 12px;
    margin-top: 12px;
    align-items: center;
}


.selec-photos img {
    width: 20px;
}

.adpt {
    display: flex;
    background-color: #BCBCBC;
    width: 140px;
    height: 140px;
    justify-content: center;
    align-items: center;
    border-radius: 15px;
}

.more {
    margin-left: 12px;
    background-color: #BCBCBC;
    color: #193083;
    border: none;
    border-radius: 50px;
    width: 30px;
    height: 30px;
}

.right-content {
    display: flex;
    flex-direction: column;
    gap: 50px;
    align-items: center;
    margin-left: 30px;
}

.ad-title {
    text-align: left;
    gap: 10px;
}

.titulo {
    font-size: 28px;
    font-style: normal;
    font-weight: 400;
    max-width: 40vw;
}

.data-post {
    color: #0148FF;
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
}

.ad-code {
    color: #0148FF;
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
}

.price {
    display: flex;
    flex-direction: column;
    align-items: center;
}

.valor {
    color: #0019FE;
    font-size: 30px;
    font-style: normal;
    font-weight: 900;
    margin: 0;
}

.entrada {
    color: #0019FE;
    font-size: 18px;
    font-style: normal;
    font-weight: 500;
    line-height: normal;
    margin: 0;
}

.contact {
    border: solid 3px #193083;
    border-radius: 30px;
    color: #193083;
    width: 240px;
    padding: 20px;
    font-size: 20px;
    font-style: normal;
    font-weight: 500;
    margin-top: 10px;
    margin-bottom: 10px;
    cursor: pointer;
    text-align: center;
    text-decoration: none;
}

.simulation {
    color: #0148FF;
    font-size: 15px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

.contact i {
    margin-right: 8px;
}

.info-sec {
    font-size: 25px;
    font-style: normal;
    font-weight: 700;
    line-height: normal;
    margin-top: 20px;
}

.descrip-sec {
    font-size: 20px;
    font-style: normal;
    font-weight: 400;
    width: 90vw;
    text-align: left;
}

.rooms {
    display: flex;
    flex-direction: column;
    margin-top: 8px;
}

.rooms-icons {
    display: flex;
    flex-direction: row;
    gap: 40px;
    margin-top: 10px;
}

.room-info {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
}

.room-info p {
    font-size: 20px;
    font-style: normal;
    font-weight: 400;
}

.add-rooms {
    display: flex;
    flex-direction: column;
    margin-top: 8px;
    justify-content: center;
}

.additional {
    padding: 10px;
    border-radius: 15px;
    border: 3px solid #A5A5A5;
    display: flex;
    flex-direction: row;
    margin-top: 8px;
    background-color: #EAEAEA;
    gap: 50px;
    align-items: center;
    justify-content: center;
    height: 150px;
    width: 600px;
}

.additional label {
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    margin-left: 5px;
}

.col-1 {
    display: flex;
    flex-direction: column;
}

.col-2 {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}


.col-3 {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

.checkbox {
    display: flex;
    flex-direction: row;
    gap: 5px;
    align-items: center;
    justify-content: center;
}

.map-sec {
    display: flex;
    flex-direction: row;
}

.left-map img {
    margin-top: 10px;
}

.local {
    display: flex;
    flex-direction: column;
    justify-content: center;
    gap: 3px;
    margin-left: 15px;
}

.local-descrip {
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
}

.bottom-buttons {
    display: flex;
    flex-direction: row;
    justify-content: center;
    margin-top: 30px;
    gap: 50px;
}

#ad-button {
    display: flex;
    border: solid 3px #193083;
    border-radius: 30px;
    color: #193083;
    width: 240px;
    padding: 20px;
    justify-content: center;
    align-items: center;
    font-size: 20px;
    font-style: normal;
    font-weight: 500;
    margin-right: 10px;
    gap: 10px;
}

#ad-button:hover {
    background-color: #193083;
    color: white;
    border: none;
    transition: 0.8s all ease;
}

.contact:hover {
    background-color: #193083;
    color: white;
    border: none;
    transition: 0.8s all ease;
}
</style>