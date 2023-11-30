<template>
    <body>
        
    </body>
    <navbar></navbar>
    <main>
        <div class="condiv">
            <img src="../images/confirmbt.png">
            <h1>Sucesso! <br> Agora entraremos na fase de verificação, seu imóvel estará na loja em até 48h</h1>
            <a href="/">Clique aqui para voltar ao inicio!</a>
        </div>

        <FooterComp/>
    </main>
</template>

<style scoped>
    @import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

    * {
        font-family: 'Poppins', sans-serif;
    }

    body {
        margin: 0;
        padding: 0;
        overflow-x: hidden;
    }

    .condiv {
        display: flex;
        justify-content: center;
        align-items: center;
        width: 100vw;
        height: 100vh;
        flex-direction: column;
        text-align: center;
    }
</style>