<template>
  <footer>
    <div class="footer-content">
      <div class="contato">
        <h3>Contato</h3>
        <p>Telefone: (21) 9999-9999</p>
        <p>E-mail: contato@petchatflow.com</p>
        <p>Endereço: Rua dos Pets, 123</p>
        <p>Horário: Seg-Sáb, 9h-19h</p>
      </div>
      <div class="redes-sociais">
        <h3>Siga-nos</h3>
        <a href="#" target="_blank"><i class="fab fa-facebook"></i></a>
        <a href="#" target="_blank"><i class="fab fa-instagram"></i></a>
        <a href="#" target="_blank"><i class="fab fa-twitter"></i></a>
      </div>
    </div>
    <div class="copyright">
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
</style>
