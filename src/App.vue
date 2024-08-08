<template>
  <main>
    <section class="login-container">
      <div class="container login">
        <texto> Comece agora sua jornada no mundo <marrom>dev,</marrom> faça agora seu login e aproveite nosso curso <marrom>gratuito!</marrom></texto>
        <div class="caixa">
          <img src="./assets/foguete.svg" alt="Foguete" />
          <div class="inputsbx">
            <input type="text" placeholder="username" />
            <input :type="isVisibly ? 'text' : 'password'" placeholder="password"/>
              <div class="esq_senha">Esqueceu sua senha?</div>
          </div>
          <div class="botoes">
            <button class="partir">Partir</button>
            <div class="cadastre-se">Cadastre-se ></div>
          </div>
        </div>
      </div>
    </section>
  </main>
</template>

<script>
export default {
  data() {
    return {
      username: "",
      isVisibly: true,
    };
  },
};
</script>

<style scoped>
body {
  height: 100%;
}
main {
  height: 100%;
}
.login-container {
  height: 100%;
  background-image: url("./assets/star-trails.svg");
  background-size: cover;
  font-family: "Rubik";
}
.login {
  padding: 180px 79px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
texto {
  color: white;
  max-width: 682px;
  font-weight: 700;
  font-size: 3.125rem;
  line-height: 59.25px;
}
.caixa {
  padding: 54px 40px;
  font-family: "Exo";
  border-radius: 10px;
  background-color: #1f2635;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 36px;
}
.inputsbx {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 11px;
}
input {
  border: none;
  background-color: #2d3545;
  border-radius: 4px;
  min-width: 273px;
  padding: 15px 16px;
  color: #c8a585;
  font-weight: 600;
  font-size: 0.72rem;
}
.esq_senha {
  font-family: "Exo";
  font-weight: 550;
  font-size: 0.700rem;
  color: #c8a585;
}
.botoes {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 16px;
}
.partir {
  border: none;
  border-radius: 3px;
  font-family: "Exo";
  background-color: #2d3545;
  min-width: 156px;
  padding-bottom: 12px;
  padding-top: 14px;
  font-weight: 710;
  font-size: 0.873rem;
  color: #c8a585;
  cursor: pointer;
}
.cadastre-se {
  color: #c8a585;
  font-size: 12px;
  font-weight: 600;
  cursor: pointer;
  margin-left: 245px;
}
marrom {
  color: #c8a585;
}
#app {
  min-height: 100%;
}
</style>
