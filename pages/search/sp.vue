<template>
    <body> 
    </body>

    <navbar/>
    <main>
        <h1>Mostrando resultados para: São Paulo (estado)</h1>
        <div class="content">
        

        <div class="ad-card">
            <div class="anuncio-wrapper">

                <div class="ad-photo">
                    <img src="../../images/casa1.jpg" style="color: #bcbcbc;" />
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
                            <img src="../../images/vector.svg" alt="heart" class="imgad">
                        </div>
                    </div>
                    <div class="ad-content-right">
                        <h4>R$ 654.000</h4>
                        <p>R$ 196.200</p>
                    </div>
                </div>
            </div>
            </div>
            <h2>Fim! Acabou por aqui</h2>
        </div>

        <footerComp></footerComp>
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

.content {
    width: 100vw;
    height: 80vh;
}

.content h2 {
    display: flex;
    width: 100%;
    height: 100%;
    justify-content: center;
    align-items: center;
    color: #888;
}

</style>