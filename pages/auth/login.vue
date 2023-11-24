<script setup>
    const client = useSupabaseClient();
    const email = ref("");
    const password = ref('');
    const errorMsg = ref('');
    const sucessMsg = ref('');

    async function signIn() {
        try {
            const { data, error } = await client.auth.signInWithPassword({
                email: email.value,
                password: password.value,
            });
            if (error) throw error;
            sucessMsg.value = "Sucesso! Clique aqui para ir para o site!";
        } catch (error) {
            errorMsg.value = error.message;
        }
    }
</script>

<template>
    <body>
            <div class="backgroundd">
            </div>
            <main>
                <div class='card'>
                    <div class="wrapper">
                      <form @submit.prevent="signIn()">
                        <img src='../../images/logo azul.png' class="logo" />
                        <div class="errormsg">
                            {{ errorMsg }}
                        </div>
                        <div class="sucessmsg">
                            <a href="/">
                                {{ sucessMsg }}
                            </a>
                        </div>
                        <input name="email" v-model="email" id='email' placeholder='Email' class='box' required/>
                        <input name="password" v-model="password" type="password" placeholder='Senha' class='box' required/>
                        <div class="ckbox">
                            <div class="checkboxdiv">
                              <div class="ckbb">
                                <input type="checkbox" class='ckb' name='ckb'/>
                                <label htmlFor="ckb">LEMBRE DE MIM</label>
                              </div>
                              <div class="regisbt">
                                <a href='/auth/register'>CADASTRAR</a> 
                              </div>
                            </div>
                        </div>
                        <button href="/sobre" class='login'>ENTRAR</button>
                        <Messages/>
                      </form>
                    </div>
                </div>
            </main>
            </body>
</template>

<script setup>

</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

* {
    font-family: 'Poppins', sans-serif;
    padding: 0;
    margin: 0;
    box-sizing: content-box;
}

.errormsg {
    color: red;
}

.sucessmsg {
    color: green;
}

body {
    overflow-x: hidden;
    overflow-y: hidden;
}

.logo {
    width: 500px;
}

.backgroundd {
    background-image: url("../../images/background.png");
    background-size: 100vw 100vh;
    z-index: -1;
    position: fixed;
    width: 100vw;
    height: 100vh;
    background-repeat: no-repeat;
}

main {
    width: 100vw;
    height: 100vh;
}

.card {
    display: flex;
    justify-content: center;
    width: 100%;
    height: 100%;
    align-items: center;
    box-shadow: 5px 4px 10px 0px rgba(0, 0, 0, 0.25);
}

form {
    padding: 40px;
    background: #fff;
    min-width: 80%;
    min-height: 80%;
    max-width: 90%;
    max-height: 90%;
    border-radius: 20px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 12px;
    box-shadow: 0 0 20px #000;
}

.box {
    min-width: 35vw;
    min-height: 7vh;
    border-radius: 10px;
    background: #DFDFDF;
    font-weight: 900;   
    outline: none;
    border: none;
    padding: 0 0 0 10px;
    padding-left: 40px;
    font-family: Poppins;
    font-size: 14px;
    font-style: normal;
    font-weight: 900;
    line-height: normal;
}

.box::placeholder {
    color: #BCBCBC;
    font-family: Poppins;
    font-size: 14px;
    font-style: normal;
    font-weight: 900;
    line-height: normal;
}

.login {
    outline: none;
    background: #fff;
    border: solid #193083;
    padding: 10px;
    color: #193083;
    border-radius: 30px;
    padding: 20px;
    padding-left: 50px;
    padding-right: 50px;
    font-weight: 900;
    transition: .2s;
    cursor: pointer;
}

.login:hover {
    background: #193083;
    color: #fff;
    transition: .2s;
}

.login:active {
    padding: 30px;
    padding-left: 60px;
    padding-right: 60px;
    transition: .1s;
}

.ckbox {
    width: 100%;
    display: flex;
    color: #193083;
    justify-content: space-between;
}

.ckb {
    outline: none;
    border: solid white;
    content: "";
    fill: #193083;
    color: cyan;
    background: #414141;
}

.checkboxdiv {
    width: 100%;
    display: flex;
    justify-content: space-between;
}

a {
    text-decoration: none;
    text-transform: uppercase;
    color: #193083;
}

.ckbb {
    display: flex;
    justify-content: center;
    gap: 10px;
}
</style>