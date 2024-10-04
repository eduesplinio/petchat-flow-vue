<template>
  <div class="produto-card">
    <img :src="produto.imagem" :alt="produto.nome" />
    <h3>{{ produto.nome }}</h3>
    <p class="preco">R$ {{ produto.preco.toFixed(2) }}</p>
    <button>Adicionar ao Carrinho</button>
  </div>
</template>

<script>
export default {
  name: "ProdutoCard",
  props: {
    produto: {
      type: Object,
      required: true,
    },
  },
};
</script>

<style scoped>
.produto-card {
  background-color: white;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  padding: 1rem;
  text-align: center;
  transition: transform 0.3s;
}

.produto-card:hover {
  transform: translateY(-5px);
}

.produto-card img {
  width: 100%;
  height: 200px;
  object-fit: cover;
  border-radius: 8px;
  margin-bottom: 1rem;
}

h3 {
  font-size: 1.25rem;
  color: #333;
}

.preco {
  font-weight: bold;
  color: #42b983;
  margin-bottom: 1rem;
}

button {
  background-color: #42b983;
  color: white;
  border: none;
  padding: 0.5rem 1rem;
  border-radius: 4px;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

button:hover {
  background-color: #3aa876;
}
</style>
