<template>
  <section>
    <picture class="nft-picture">
      <source setsrc="./assets/image-equilibrium.jpg">
      <img src="./assets/image-equilibrium.jpg" alt="imagem da nft equilibrium">
    </picture>

    <div class="description">
      <h3>Equilibrium #3429</h3>
      <p>Our Equilibrium collection promotes balance and calm.</p>
      <div class="preco-time">
        <div>
          <img class="icone-nft" src="./assets/icon-ethereum.svg" alt="icone da nft">
          <p class="price">0.041 ETH</p>
        </div>
        <div>
          <img class="icone-tempo" src="./assets/icon-clock.svg" alt="icone de tempo">
          <p class="time">3 days left</p>
        </div>
      </div>
    </div>

    <div class="owner">
      <picture class="owner-perfil">
        <source setsrc="./assets/image-avatar.png">
        <img src="./assets/image-avatar.png" alt="perfil do criador">
      </picture>

      <p>
        Creation of <span>Jules Wyvern</span>
      </p>
    </div>

  </section>
  <div class="frontendmentor">
    <p>Challenge by Frontend Mentor. Coded by <span> Renato Vieira.</span></p>
    <img class="logo-vue" src="./assets/logo.png" alt="logo vue">
  </div>
</template>

<script>

export default {
  name: 'App',

}
</script>

<style>
:root {

  --paragrafos: hsl(215, 51%, 70%);
  --nft-price-color: hsl(178, 100%, 50%);
  --mainBG: hsl(217, 54%, 11%);
  --cardBG: hsl(216, 50%, 16%);
  --line: hsl(215, 32%, 27%);
  --Titulo: hsl(0, 0%, 100%);
  --font-size-paragrafo: 18px;
}


#app {
  font-family: 'Outfit', sans-serif;
  font-family: 'Ubuntu', sans-serif;
  text-align: center;
  color: #1363b3;
  margin-top: 60px;
}

h3 {
  color: var(--Titulo);
}

p {
  font-size: var(--font-size-paragrafo);
  color: var(--paragrafos);
}

.price {
  color: var(--nft-price-color);
}

.time {
  color: var(--paragrafos);
}

body {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background-color: var(--mainBG);
  gap: 20px;
}

section {

  display: flex;
  flex-direction: column;
  width: 300px;
  height: 550px;
  background-color: var(--cardBG);
  padding: 20px;
  justify-content: center;
  border: solid 20px var(--mainBG);
  box-shadow: 0px 9px 17px 12px var(--mainBG);
  border-radius: 20px;
}

.nft-picture {

  display: flex;
  border-radius: 10px;
  height: 300px;
  width: 300px;
}

.nft-picture img {

  display: flex;
  height: 100%;
  width: 100%;
  border-radius: 10px;
}

.description {

  display: flex;
  flex-direction: column;
  justify-content: left;
  text-align: left;
  height: 180px;
  border-bottom: solid 1px var(--line);
  margin-bottom: 20px;
  padding-bottom: 20px;
}

.preco-time {

  display: flex;
  flex-direction: row;
  justify-content: space-between;
}

.preco-time div {

  display: flex;
  flex-direction: row;
  align-items: center;
  gap: 5px;
}

.icone-tempo {

  display: flex;
  width: 20px;
  height: 20px;
}

.owner {

  display: flex;
  flex-direction: row;
  gap: 20px;
  align-items: center;
  padding-top: 10px;
  padding-bottom: 20px;
  height: 12px;

}

.owner picture {

  display: flex;
  width: 30px;
  height: 30px;
}

span {

  color: var(--Titulo);
}

.logo-vue {

  display: flex;
  width: 30px;
  height: 30px;
}

.frontendmentor {
  display: flex;
  flex-direction: row;
  gap: 5px;
  align-items: center;
}


@media(max-width: 376px) {
  
  section{

    display: flex;
    align-items: start;
  }
}

</style>
