<template>
  <div>
    <div>
      <p>Junte-se à nossa turma de <strong> {{ leitores }} leitores ativos</strong>.</p>
    </div>
    <form>
      <label for="endereco_email">
        <span>
          <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-envelope"
            viewBox="0 0 16 16">
            <path
              d="M0 4a2 2 0 0 1 2-2h12a2 2 0 0 1 2 2v8a2 2 0 0 1-2 2H2a2 2 0 0 1-2-2V4Zm2-1a1 1 0 0 0-1 1v.217l7 4.2 7-4.2V4a1 1 0 0 0-1-1H2Zm13 2.383-4.708 2.825L15 11.105V5.383Zm-.034 6.876-5.64-3.471L8 9.583l-1.326-.795-5.64 3.47A1 1 0 0 0 2 13h12a1 1 0 0 0 .966-.741ZM1 11.105l4.708-2.897L1 5.383v5.722Z" />
          </svg>
        </span>
        <input type="email" name="endereco_email" id="endereco_email" placeholder="Seu email principal">
      </label>

      <button type="submit" class="submit-btn"> Increver-se (Grátis)</button>
    </form>
  </div>
</template>

<script>
export default {
  name: 'FormularioInscricao',
  props: {
    leitores: String
  }
}
</script>

<style scoped>

label {
  width: 100%;
  display: flex;
  padding: 10px 15px;
  border: 1px solid #ccc;
  border-radius: 5px;
  align-items: center;
  gap: 15px;
  margin: 15px 0;
}

label:focus {
  border: 1px solid #000;
}

label span {
  margin-right: 5px;
}

input {
  width: 100%;
  border: 0;
  font-size: 1em;
  font-weight: lighter;
  padding: 10px 0;
 }

 input:focus {
  outline: 0;
 }

 button {
  width: 100%;
  padding: 20px 25px;
  color: #FFFFFF;
  background-color: #0070f3;
  border: 0;
  border-radius: 5px;
  font-size: 1.2em;
  -webkit-box-shadow: 0 6px 20px rgba(0,118,255,.23);
  -moz-box-shadow: 0 6px 20px rgba(0,118,255,.23);
  box-shadow: 0 6px 20px rgba(0,118,255,.23);
 }

 button:hover {
    background: rgba(0,118,255,.9);
 }
</style>
