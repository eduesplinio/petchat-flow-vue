---
description: 'Para configurar o projeto localmente, siga os passos abaixo:'
icon: gear
---

# Configuração do Projeto

1\. Clonar o Repositório

Clone o repositório para o seu ambiente de desenvolvimento:

```bash
git clone https://github.com/SEU_USUARIO/petflow-chat-frontend.git
cd petflow-chat-frontend
```

#### 2. Instalar Dependências

Instale todas as dependências necessárias para o funcionamento da aplicação:

```bash
npm install
# ou
yarn install
```

#### 3. Executar a Aplicação

Inicie o servidor de desenvolvimento para rodar a aplicação localmente:

```bash
npm run serve
# ou
yarn serve
```

A aplicação estará disponível em [http://localhost:8080](http://localhost:8080).

### Estrutura de Diretórios

Aqui está uma visão geral da estrutura do projeto:

```bash
petflow-chat-frontend/
├── public/                 # Arquivos públicos e index.html
├── src/
│   ├── assets/             # Recursos como imagens e estilos
│   ├── components/         # Componentes Vue.js reutilizáveis
│   ├── views/              # Páginas principais da aplicação
│   ├── store/              # Gerenciamento de estado Vuex
│   └── App.vue             # Componente raiz da aplicação
├── babel.config.js         # Configurações do Babel
├── package.json            # Dependências e scripts do projeto
└── vue.config.js           # Configurações personalizadas do
```
