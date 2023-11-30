<template>
    <div class="ad-card">
            <div class="anuncio-wrapper">

                <div class="ad-photo">
                    <img src="svg/photo.png" style="color: #bcbcbc;" />
                </div>
                <div class="ad-content">
                    <div class="ad-content-left">
                        <div class="ad-content-left-top">
                            <h2>Título do anúncio</h2>
                            <p>Bairro, Cidade</p>
                        </div>
                        <div class="ad-content-left-middle">
                            odase
                        </div>
                        <div class="ad-content-left-bottom">
                            <img src="svg/heart.png" alt="heart">
                        </div>
                    </div>
                    <div class="ad-content-right">
                        <h4>R$ VALOR DO TOTAL</h4>
                        <p>VALOR DA ENTRADA</p>
                    </div>
                </div>
            </div>
        </div>
</template>

<style scoped>
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
    width: 85px;
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
    width: 30%;
    display: flex;
    justify-content: flex-end;
    flex-direction: column;
}

.ad-content-right h4 {
    font-weight: 500;
    color: #193083;
    font-size: 1.2rem;
}

.ad-content-right p {
    font-weight: 400;
    font-size: 0.92rem;
    margin-left: 40px;
}

.ad-content-left-bottom img {
    width: 25px;
    margin: 10px;
}
</style>