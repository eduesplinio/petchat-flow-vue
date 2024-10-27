<template>
  <footer class="footer">
    <div class="footer-content">
      <div class="footer-section links">
        <h3>Links Úteis</h3>
        <ul>
          <li><a href="#servicos">Serviços</a></li>
          <li><a href="#produtos">Produtos</a></li>
          <li><a href="#contato">Contato</a></li>
        </ul>
      </div>
      <div class="footer-section contato">
        <h3>Contato</h3>
        <p>Telefone: (21) 9999-9999</p>
        <p>E-mail: contato@petchatflow.com</p>
        <p>Endereço: Rua dos Pets, 123</p>
        <p>Horário: Seg-Sáb, 9h-19h</p>
      </div>
      <div class="footer-section redes-sociais">
        <h3>Siga-nos</h3>
        <a href="#" target="_blank"><i class="fab fa-facebook"></i></a>
        <a href="#" target="_blank"><i class="fab fa-instagram"></i></a>
        <a href="#" target="_blank"><i class="fab fa-twitter"></i></a>
      </div>
    </div>
    <div class="footer-bottom">
      <p>&copy; 2024 PetChatFlow. Todos os direitos reservados.</p>
    </div>
  </footer>
</template>

<script>
export default {
  name: "FooterView",
};
</script>

<style scoped>
footer {
  background-color: #333;
  color: white;
  padding: 2rem;
  width: 100%;
  z-index: 1000;
  position: relative; /* Adicionado para garantir que o rodapé fique no final */
  margin-top: -200px;
  bottom: 0;
}

.footer-content {
  display: flex;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
}

.contato {
  max-width: 300px;
}

.contato h3 {
  margin-bottom: 1rem;
  font-size: 1.5rem;
}

.contato p {
  margin: 0.5rem 0;
  line-height: 1.5;
}

.redes-sociais a {
  color: white;
  font-size: 1.5rem;
  margin-right: 1rem;
}

.copyright {
  text-align: center;
  margin-top: 2rem;
  font-size: 0.9rem;
}

.footer {
  background-color: #333;
  color: #fff;
  padding: 2rem 0;
  text-align: center;
}

.footer-content {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  max-width: 1200px;
  margin: 0 auto;
}

.footer-section {
  flex: 1;
  margin: 1rem;
  min-width: 200px;
}

.footer-section h3 {
  margin-bottom: 1rem;
}

.footer-section p,
.footer-section ul {
  margin: 0;
  padding: 0;
  list-style: none;
}

.footer-section p {
  margin-bottom: 1rem; /* Adicionado mais espaçamento entre os parágrafos */
}

.footer-section ul li {
  margin-bottom: 0.5rem;
}

.footer-section ul li a {
  color: #fff;
  text-decoration: none;
}

.footer-section ul li a:hover {
  text-decoration: underline;
}

.footer-section .redes-sociais a {
  color: #fff;
  margin: 1rem; /* Ajustado o espaçamento entre os ícones */
  font-size: 1.5rem;
  transition: transform 0.3s, color 0.3s; /* Adicionado efeito de transição */
}

.footer-section .redes-sociais a:hover {
  color: #1da1f2; /* Cor azul moderna */
  transform: scale(1.2); /* Efeito de escala ao passar o mouse */
}

.footer-bottom {
  margin-top: 2rem;
  border-top: 1px solid #444;
  padding-top: 1rem;
}
</style>
