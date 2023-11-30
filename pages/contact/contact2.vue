<template>
    <body></body>
    <navbar/>
    <main>
        <div class="content">
            <div class="name">
                <h1> CASA EM CONDOMINIO FECHADO PARA ALUGAR! </h1>
            </div>
            <div class="contact">
                <h1>WhatsApp: +55 (21) 98345-4219 - Vendedor Teste 1</h1>
            </div>
        </div>
        <footerComp></footerComp>
    </main>
</template>

<style scoped>
    @import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

    * {
        font-family: "Poppins", sans-serif;
        margin: 0;
        padding: 0px;
    }

    body {
        margin: 0;
        padding: 0;
    }

    .content {
        display: flex;
        align-items: center;
        justify-content: center;
        flex-direction: column;
        gap: 200px;
        width: 100vw;
        height: 80vh;
    }
</style>