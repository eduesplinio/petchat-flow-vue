<template>
  <div class="servico-card">
    <i :class="['fas', servico.icone]"></i>
    <h3>{{ servico.nome }}</h3>
  </div>
</template>

<script>
export default {
  name: "ServicoCard",
  props: {
    servico: Object,
  },
};
</script>

<style scoped>
.servico-card {
  background-color: #f5f5f5;
  border-radius: 8px;
  padding: 2rem;
  text-align: center;
  transition: transform 0.3s ease;
}

.servico-card:hover {
  transform: translateY(-5px);
}

.servico-card i {
  font-size: 3rem;
  color: #42b983;
  margin-bottom: 1rem;
}
</style>
