<template>
    <body class="bodik"></body> 
    <main>
        <navbar/>
        <div class="anunciar">
            <div class="texts">
                <h1 class="tx1">Vamos anúnciar seu </h1> <h1 class="tx2"> IMÓVEL!</h1>
            </div>
            <div class="type">
                <div class="center-select">
                    <input type="radio" name="tipo-imovel" id="Destaque">
                    <label for="Destaque">Vender</label>

                    <input type="radio" name="tipo-imovel" id="Todos">
                    <label for="Todos">Alugar</label>

                    <input type="radio" name="tipo-imovel" id="Temporada">
                    <label for="Temporada">Temporada</label>
                </div>
            </div>
        </div>

        <div class="select">
            <input type="file" class="selectdiv" id="file" name="file">
            <label for="file" class="filelabel">Clique para enviar as imagens aqui</label>
            <img class="imageen" src="../images/sent.svg" alt="">
        </div>

        <form>
            <label class="labelinput" for="nomeanuncio">Título do anúncio:</label>
            <input class="forminput" type="text" id="nomeanuncio" placeholder="Ex: Casa de praia localizada no litora norte de SP...">
            <label class="labelinput" for="descanuncio">Descrição:</label>
            <input class="forminput" type="text" id="descanuncio" placeholder="Ex: Casa grande e confortável ideal para sua família...">

            <label class="filter-box-label" for=""> Áreas adicionais: </label>
                    <div class="filter-box">
                        <div class="conteiner">
                            <div>
                                <input type="checkbox" name="filtro" id="Piscina">
                                <label for="Piscina">Piscina</label>
                            </div>

                            <div>
                                <input type="checkbox" name="filtro" id="Sauna">
                                <label for="Sauna">Sauna</label>
                            </div>

                            <div>
                                <input type="checkbox" name="filtro" id="Academia">
                                <label for="Academia">Academia</label>
                            </div>
                            
                            <div>
                                <input type="checkbox" name="filtro" id="Quadra">
                                <label for="Quadra">Quadra</label>
                            </div>

                            <div>
                                <input type="checkbox" name="filtro" id="Espaço pet<">
                                <label for="Espaço pet<">Espaço pet</label>
                            </div>
                        </div>

                        <div class="conteiner">
                            <div>
                                <input type="checkbox" name="filtro" id="Espaço gourmet">
                                <label for="Espaço gourmet">Espaço gourmet</label>
                            </div>

                            <div>
                                <input type="checkbox" name="filtro" id="Forno para pizza">
                                <label for="Forno para pizza">Forno para pizza</label>
                            </div>

                            <div>
                                <input type="checkbox" name="filtro" id="Churrasqueira">
                                <label for="Churrasqueira">Churrasqueira</label>
                            </div>

                            <div>
                                <input type="checkbox" name="filtro" id="Horta">
                                <label for="Horta">Horta</label>
                            </div>

                            <div>
                                <input type="checkbox" name="filtro" id="Salão de festas">
                                <label for="Salão de festas">Salão de festas</label>
                            </div>
                        </div>
                        
                        <div class="conteiner">
                            <div>
                                <input type="checkbox" name="filtro" id="Brinquedoteca">
                                <label for="Brinquedoteca">Brinquedoteca</label>
                            </div>

                            <div>
                                <input type="checkbox" name="filtro" id="Playground">
                                <label for="Playground">Playground</label>
                            </div>

                            <div>
                                <input type="checkbox" name="filtro" id="Espaço para leitura">
                                <label for="Espaço para leitura">Espaço para leitura</label>
                            </div>

                            <div>
                                <input type="checkbox" name="filtro" id="Cinema pessoal">
                                <label for="Cinema pessoal">Cinema pessoal</label>
                            </div>

                            <div>
                                <input type="checkbox" name="filtro" id="Salão de jogos">
                                <label for="Salão de jogos">Salão de jogos</label>
                            </div>
                        </div>
                    </div>    
                    
                    <div class="top-info">
                        <div class="label">
                            <label for="m2">Área útil (m2)</label>
                            <input type="text" class="m2" id="m2">
                        </div>
                        <div class="label">
                            <label for="ban">Banheiros</label>
                            <input type="text" class="ban" id="ban">
                        </div>
                        <div class="label">
                            <label for="qua">Quartos</label>
                            <input type="text" class="qua" id="qua">
                        </div>
                        <div class="label">
                            <label for="and">Andares</label>
                            <input type="text" class="and" id="and">
                        </div>
                        <div class="label">
                            <label for="va">Vagas</label>
                            <input type="text" class="va" id="va">
                        </div>
                    </div>
                    <div class="bottom-info">
                        <div class="label">
                            <label for="ipt">IPTU (R$)</label>
                            <input type="text" class="ipt" id="ipt">
                        </div>
                        <div class="label">
                            <label for="con">Condomínio (R$)</label>
                            <input type="text" class="con" id="con">
                        </div>
                        <div class="label">
                            <label for="ent">Entrada (R$)</label>
                            <input type="text" class="ent" id="ent">
                        </div>
                        <div class="label">
                            <label for="vt">Valor total (R$)</label>
                            <input type="text" class="vt" id="vt">
                        </div>
                    </div>

                    <div class="addinfo">
                        <label for="addinf">Informações adicionais</label>
                        <input type="text" id="addinf" class="addinf">
                    </div>

                    <div class="top-info">
                        <div class="label">
                            <label for="brr">BAIRRO</label>
                            <input type="text" class="brr" id="brr">
                        </div>
                        <div class="label">
                            <label for="cdd">CIDADE</label>
                            <input type="text" class="cdd" id="cdd">
                        </div>
                    </div>
                    <div class="bottom-info">
                        <div class="label">
                            <label for="cep">CEP</label>
                            <input type="text" class="cep" id="cep">
                        </div>
                        <div class="label">
                            <label for="end">ENDEREÇO</label>
                            <input type="text" class="end" id="end">
                        </div>
                        <div class="label">
                            <label for="uf">UF</label>
                            <input type="text" class="uf" id="uf">
                        </div>
                    </div>

                    <h4>Aceita FGTS?</h4>
                    <div class="consult">
                        <div class="radio">
                            <input type="radio" class="fgts" name="fgts" id="fgts">
                            <label for="fgts">Sim</label>
                        </div>
                        <div class="radio">
                            <input type="radio" class="fgts2" name="fgts" id="fgts2">
                            <label for="fgts2">Não</label>
                        </div>
                    </div>

                    <div class="termos">
                        <input type="checkbox">
                        <p>Concordo com os </p>
                        <a href="/terms" target="_blank">termos de uso</a>
                    </div>

                    <a href="/confirm" class="cobut"> CRIAR <br> ANÚNCIO </a>
        </form>

        <footerComp/>
    </main>
</template>

<style scoped>
    @import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

    * {
        font-family: 'Poppins', sans-serif;
    }

    .filter-box-label {
        margin-top: 50px;
    }

    .top-info {
        display: flex;
        width: 100vw;
        flex-direction: row;
        justify-content: center;
        margin-bottom: 50px;
        margin-top: 50px;
        gap: 20px;
    }

    .termos {
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;
        gap: 5px;
    }

    .cobut {
        text-decoration: none;
        font-weight: 600;
        text-align: center;
        border: 2px solid #193083;
        border-radius: 30px;
        padding: 0px 30px 0px 30px;
        margin-bottom: 20px;
        transition: .2s;
    }

    .cobut:hover {
        background: #193083;
        color: #fff;
        transition: .2s;
    }

    .bottom-info {
        display: flex;
        width: 100vw;
        flex-direction: row;
        justify-content: center;
        gap: 20px;
    }

    .label {
        display: flex;
        flex-direction: column;
    }

    .consult {
        display: flex;
        gap: 20px;
    }

    .label input {
        width: 80%;
        border: 1px solid #A5A5A5;
        padding: 20px 15px 20px 15px;
        border-radius: 20px;
        outline: none;
    }

    .addinfo {
        display: flex;
        flex-direction: column;
    }

    .addinfo input {
        width: 80vw;
        border: 1px solid #A5A5A5;
        padding: 20px 15px 20px 15px;
        border-radius: 20px;
        outline: none;
    }

    .bodik {
        margin: 0;
        overflow-x: hidden;
    }

    .imageen {
        position: absolute;
        top: 300px;
    }

    .center-select {
    margin: 15px;
}
    .bottom-select {
    margin: 15px;
}

    .texts {
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: row;
        gap: 10px;
    }

    .type {
        display: flex;
        align-items: center;
        justify-content: center;
    }
    
    .tipo {
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .tx2 {
        color: #193083;
    }

    .center-select input[type="radio"] {
        opacity: 0;
        position: fixed;
        width: 0;
    }

    .center-select label {
        display: inline-block;
        padding: 10px 20px;
        font-family: sans-serif, Arial;
        font-size: 16px;
        transition: 0.2s;
    }

    .center-select label:hover {
        border-bottom: 4px solid #19308377;
        transition: 0.2s;

    }

    .center-select input[type="radio"]:checked+label {
        border-bottom: 4px solid #193083;
    }

    .center-select input[type="radio"] {
        opacity: 0;
        position: fixed;
        width: 0;
    }

    .center-select label {
        display: inline-block;
        padding: 10px 20px;
        font-family: sans-serif, Arial;
        font-size: 16px;
        transition: 0.2s;
    }

    .center-select label:hover {
        border-bottom: 4px solid #19308377;
        transition: 0.2s;

    }

    .center-select input[type="radio"]:checked+label {
        border-bottom: 4px solid #193083;
    }

    .select {
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .selectdiv {
        display: none;
    }

    .filelabel {
        display: block;
        cursor: pointer;    
        background: #EDEDED;
        padding: 120px 120px 80px 120px;
        font-weight: 600;
        font-size: 1.4rem;
        color: #193083;
        border-radius: 24px;
    }
    
    form {
        display: flex;
        width: 100vw;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        overflow: hidden;
    }

    .forminput {
        display: flex;
        justify-content: center;
        align-items: center;
        width: 80%;
        border: 1px solid #A5A5A5;
        padding: 20px 15px 20px 15px;
        border-radius: 20px;
        outline: none;
    }

    .labelinput {
        width: 80vw;
        display: flex;
        justify-content: flex-start;
    }

    .filter-box {
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;
        width: 50vw;
        height: 30vh;
        background: #EAEAEA;
        gap: 150px;
        border-radius: 20px;
        border: 2px solid #A5A5A5;
        margin-bottom: 50px;
    }

    .conteiner {
        display: flex;
        flex-direction: column-reverse;
        gap: 10px;
    }

</style>