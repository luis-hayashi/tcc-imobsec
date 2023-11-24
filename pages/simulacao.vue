<template>
    <div class="backgroundd">
    </div>

    <navbar/>
    <main>
        <div class="Simu">

            <div class="card">
                
                <h1>Vamos simular a compra de seu imóvel</h1>

                <div class="box">
                    <input type="number" name="" id="" placeholder="Renda bruta mensal"/>
                    <input type="number" name="" id="" placeholder="Valor do imóvel"/>
                    <input type="number" name="" id="" placeholder="Valor de entrada"/>
                    <input type="number" name="" id="" placeholder="Tempo de pagamento (mêses)"/>
                </div>

                <button type="submit">SIMULAR</button>

            </div>
        </div>
    </main>
    <footerComp/>
</template>

<style scoped>
    @import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

* {
    font-family: 'Poppins', sans-serif;
    padding: 0;
    margin: 0;
    box-sizing: content-box;
}

.backgroundd {
    background-image: url("../images/dinheiro.png");
    background-size: 100vw 100vh;
    z-index: -1;
    position: fixed;
    width: 100vw;
    height: 100vh;
    background-repeat: no-repeat;
}

body {
    margin: 0;
    overflow-x: hidden;
}

.Simu {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: row;
    width: 100vw;
    height: 100vh;
}

.card {
    border-radius: 10px;
    border: 1px solid rgba(0, 0, 0, 0.12);
    background: #FFF;
    box-shadow: 3px 4px 6px 0px rgba(0, 0, 0, 0.28);
    display: flex;
    flex-direction: column;
    padding: 15px;
    justify-content: center;
    align-items: center;
    height: auto;
    width: 65vw;
    gap: 15px;
}

h1 {
    color: rgba(0, 0, 0, 0.64);
    font-size: 30px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    cursor: default;
}

.box {
    display: flex;
    flex-direction: column;
    gap: 20px;
    padding: 10px;

}

.box input {
    height: 50px;
    width: 50vw;
    border-radius: 10px;
    border: 1px solid rgba(0, 0, 0, 0.12);
    background: #FFF;
    box-shadow: 3px 4px 6px 0px rgba(0, 0, 0, 0.28);
}

.box input::placeholder {
    padding: 10px;
    font-weight: 400;
    color: rgba(0, 0, 0, 0.50);
}

button {
    outline: none;
    background: #fff;
    border: solid #193083;
    color: #193083;
    border-radius: 30px;
    padding: 10px;
    padding-left: 40px;
    padding-right: 40px;
    font-size: 25px;
    font-weight: 700;
    transition: .2s;
    cursor: pointer;
}

button:hover {
    background: #193083;
    color: #fff;
    transition: .2s;
}

button:active {
    padding: 20px;
    padding-left: 40px;
    padding-right: 40px;
    transition: .1s;
}
</style>