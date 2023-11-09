<template>
  <main class="container-principal">
    <div class="center">
      <img class="avatar" src="/avatar.png" alt="avatar">
      <div>
        <h1>
          Notícias de Tecnologia para quem não tem tempo de ler notícias.
        </h1>
      </div>
      <FormularioInscricao :leitores="total_incritos"/>
    </div>
  </main>
</template>

<script>
import FormularioInscricao from './components/FormularioInscricao.vue';


export default {
  name: 'App',
  components: {
    FormularioInscricao
},
data() {
  return {
    total_incritos: '112.075'
  }
}
}
</script>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, Helvetica, sans-serif;
    background-color: aliceblue;
}

h1 {
  margin: 25px auto;
  text-align: center;
}

.container-principal {
  display: flex;
  flex-direction: column;
  -ms-flex-align: center;
  align-items: center;
  margin-top: 10%;
}

.center {
  max-width: 50vw;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.avatar {
  background-color: #c4c556;
  border-radius: 50%;
  width: 100px;
  height: 100px;
  padding-top: 10px;
  margin: 20px 0;
}
</style>
