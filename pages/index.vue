<template>
    <body class="bodiis"></body>
        <navbar/>
        <main>
            <div class="apresentation">
                <div class="text-cont">
                    <h1> Sobre o iMobSec! </h1>
                    <h1> Saiba mais sobre os <br> fundadores e idealização <br> do projeto iMobSec!  </h1>
                    <h1> Confira: </h1>
                </div>
                <div class="image">
                    <img src="../images/backgg.svg">
                </div>
            </div>
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
        width: 43vw;
        gap: 20px;
        flex-direction: column;
        color: white;
        background: #193083;
        justify-content: center;
        padding-left: 20px;
    }
    
    h1 {
        font-size: 1.8rem;
        font-weight: 400;
    }
</style>