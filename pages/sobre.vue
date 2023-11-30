<template>
    <body>
        
    </body>
    <main>
    <navbar />
            
                <div class="about">
                    <div class="logo-azul">
                        <img src='../images/logo azul.png' class="image"/>
                    </div>

                    <div class="texto-1">
                        <h1 class="h1"> O que é o iMobSec? </h1>
                        <p class="p"> O iMobSec tem como finalidade ser uma plataforma eficiente no mercado imobiliário na internet, de forma democratizada, buscando entregar todos os requisitos e necessidades do usuário de forma segura e prática. Foi um projeto idealizado por quatro estudantes do curso de desenvolvimento de sistemas da ETEC de São José dos Campos, como projeto de conclusão de curso.</p>
                    </div>

                    <div class="textos-2">
                        <div class="nome">
                            <h1 class="h1">Como surgiu o nome?</h1>
                            <p class="p">Com todas as informações iniciais em mãos, decidiram o nome "iMobSec". O "i" no início vem de internet, já fazendo junção ao "Mob", fazendo referência ao termo "imóvel" em inglês, e "Sec" de "security", também do inglês, que significa segurança. Esse nome remete a tudo que o site oferece ao cliente. A partir daí, definiram sua identidade visual, problemas, resoluções, entre outros processos, até chegar ao que é hoje."</p>
                        </div>

                        <div class="ideia">
                            <h1 class="h1">De onde surgiu a ideia?</h1>
                            <p class="p">O projeto teve início em uma conversa entre os dois desenvolvedores sobre o mercado imobiliário online, pois ambos possuem familiares que trabalham na área e observavam de perto como é trabalhar nesse mercado. Decidiram, então, como tema do TCC, justamente essa área. Foram anotando as ideias principais para a plataforma que sentiam falta em outras concorrentes, e disponibilizaram pesquisas sobre os requisitos para que o público determinasse suas necessidades.</p>
                        </div>
                    </div>

                    <div class="desenvolvedores">
                        <h1 class="h1">Sobre os desenvolvedores</h1>
                    </div>

                    <div class="fabio">

                        <h1 class="h1">Fábio da Cruz Leite</h1>
                        <div class="texto-fabio">
                            <Image src='/images/perfilfoda.png' alt="img" width="150" height="150" class="profille-pic" />
                            <p class="p"></p>
                        </div>
                    </div>

                    <div class="hayashi">
                        <h1 class="h1">Luis Felipe Hayashi</h1>
                        <div class="texto-hayashi">
                            <p class="p">Sou Luis Felipe, um aluno da ETEC apaixonado por tecnologia e inovação, e estou comprometido em impulsionar a transformação positiva no mercado imobiliário por meio da minha dedicação e conhecimento. Desempenhei um papel importante no desenvolvimento da empresa iMobSec, incorporando tecnologia avançada ao setor imobiliário para criar soluções inovadoras.</p>
                            <Image src='/images/perfilfoda.png' alt="img" width="150" height="150" class="profille-pic" />
                        </div>
                    </div>

                    <div class="geron">
                        <h1 class="h1">Geron Gabriel da Silva</h1>
                        <div class="texto-geron">
                            <Image src='/images/perfilfoda.png' alt="img" width="150" height="150" class="profille-pic" />
                            <p class="p">Olá, sou Geron Gabriel da Silva Pécora, um aluno dedicado da Etec, interessado pela área de tecnologia. Desde cedo, desenvolvi um interesse profundo em programação e design de sites, o que me levou a me tornar um dos desenvolvedores-chave por trás do incrível projeto do site imobiliário iMobSec.</p>
                        </div>
                    </div>

                    <div class="ygor">
                        <h1 class="h1">Ygor Pereira</h1>
                        <div class="texto-ygor">
                            <p class="p">Ygor Ruan Pereira, nascido em 6 de janeiro de 2006, é um estudante brasileiro natural de São José dos Campos, interior do estado de São Paulo. Atualmente, ele é aluno do curso de Desenvolvimento de Sistemas na ETEC de São José dos Campos. Desde jovem, Ygor sempre teve interesse pela tecnologia e pelo mundo da programação, então ele decidiu seguir a carreira de desenvolvedor de sistemas e começou seus estudos na ETEC.  Ele é uma pessoa comunicativa e sociável, e sempre está disposto a ajudar aqueles ao seu redor.</p>
                            <Image src='/images/perfilfoda.png' alt="img" width="150" height="150" class="profille-pic" />
                        </div>
                    </div>
                </div>
                <footer>
                    <footerComp />
                </footer>
            </main>
</template>

<script setup>

</script>

<style scoped>
     @import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

* {
    font-family: 'Poppins', sans-serif;
    margin: 0;
    padding: 0;
}

body {
    padding: 0;
    margin: 0;
}

html {
    padding: 0;
    margin: 0;
    width: 100vw;
    height: 100vh;
}

template {
    margin: auto;
    width: 100vw;
    height: 100vh;
    overflow-x: hidden;
}

.about {
    display: flex;
    flex-direction: column;
    gap: 15px;

}

.logo-azul {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

.texto-1 {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    width: 100%;
    overflow: hidden;
}

.texto-1 p {
    width: 85%;
}

.textos-2 {
    display: flex;
    flex-direction: row;
    text-align: left;
    gap: 50px;
    height: 60%;
}

.ideia {
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 50%;
    text-align: right;
}

.nome {
    display: flex;
    flex-direction: column;

    align-items: center;
    width: 50%;
    text-align: left;
}

.textos-2 p {
    max-width: 75%;
}


.desenvolvedores {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

.fabio h1{
    width: 95%;
}

.fabio {
    display: flex;
    flex-direction: column;
    padding: 20px;
    text-align: right;
}

.texto-fabio {
    display: flex;
    flex-direction: row;
    max-width: 95%;
    text-align: right;
    gap: 25px;
}

.hayashi {
    display: flex;
    flex-direction: column;
    padding: 20px;
}

.texto-hayashi {
    display: flex;
    flex-direction: row;
    width: 95%;
    text-align: left;
    gap: 15px;
}

.geron {
    display: flex;
    flex-direction: column;
    padding: 20px;
    text-align: right;
}

.geron h1{
    width: 95%;
}

.texto-geron {
    display: flex;
    flex-direction: row;
    width: 95%;
    text-align: right;
    gap: 25px;
}

.ygor {
    display: flex;
    flex-direction: column;
    padding: 20px;
}

.texto-ygor {
    display: flex;
    flex-direction: row;
    width: 95%;
    text-align: left;
    gap: 10px;
}

.profille-pic{
    border-radius: 50%;
}

.h1 {
    color: #000;
    font-size: 22px;
    font-style: normal;
    font-weight: 700;
    line-height: normal;
}

.p {
    color: #000;
    font-size: 16px;
    font-style: normal;
    font-weight: 300;
    line-height: normal;
}

@media(max-width:768px){

    .image {
        width: 100%;
    }
    .about {
        display: flex;
        align-items: center;
        width: 100vw;
    }
}

</style>