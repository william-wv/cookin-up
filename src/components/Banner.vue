<script>
export default {
  name: "Banner"
}
</script>

<template>
  <header class="banner">
    <div class="apresentacao">
      <img class="logo" src="../assets/img/Logo.svg" alt="logo">

      <p class="cabecalho-lg frase-cabecalho">
        <span class="texto-verde">Um banquete de ideias para </span>despertar o chef que há em você!
      </p>

      <p class="subtitulo-lg">Explore novas receitas todos os dias com os ingredientes que estão ao seu alcance!</p>

    </div>
    <img class="fo-banner" src="../assets//img/Hero Image.png" alt="">
  </header>
</template>

<style scoped>
.banner {
  padding: 4rem 7.5rem;
  color: var(--creme);

  display: flex;
  justify-content: space-between;
  align-items: center;
  column-gap: 3.25rem;
}

.logo {
  height: 4.5rem;
  margin-bottom: 3rem;
}

.frase-cabecalho {
  margin-bottom: 2rem;
}

.texto-verde {
  color: var(--verde-medio, #3D6D4A);
}

.foto-banner {
  width: 35rem;
}


.cabecalho-lg {
  font-family: var(--cabecalhos);
  font-size: 3.35625em;
  line-height: 120%; /* 4.0275em */
}

.cabecalho {
  font-family: var(--cabecalhos);
  font-size: 2.75em;
  line-height: 120%; /* 3.3em */
}

.subtitulo-lg {
  font-size: 1.9375em;
  line-height: 150%; /* 2.90625em */
}

@media only screen and (max-width: 1300px) {
  .banner {
    padding: 4rem 3.75rem;
    flex-direction: column;
    align-items: center;
    gap: 1rem;
  }

  .logo {
    display: block;
    margin-left: auto;
    margin-right: auto;
  }
}

@media only screen and (max-width: 767px) {
  .banner {
    padding: 4rem 1.5rem;
  }

  .foto-banner {
    width: min(100%, 21.25rem);
  }
}


</style>
