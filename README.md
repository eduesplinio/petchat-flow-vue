# PetChatFlow

## Introdução
Bem-vindo ao repositório do [**PetChatFlow**](https://petflow-chat-front.vercel.app/)! Esta é a aplicação frontend desenvolvida com **Vue.js**, projetada para facilitar a comunicação eficiente dentro da plataforma Petflow. O Petflow Chat é um chatbot interativo para petshops, que utiliza a API do ChatGPT para fornecer um atendimento automatizado e amigável aos clientes de maneira eficaz.

## Ferramentas e Tecnologias Utilizadas

### **Framework Principal:** 
- **Vue.js** (^3.2.13)

### **Bibliotecas Principais:**
- [**core-js**](https://github.com/zloirock/core-js) (^3.8.3) - Polyfills para garantir compatibilidade entre diferentes navegadores.
- [**swiper**](https://swiperjs.com/) (^11.1.14) - Slider moderno e customizável para criação de interfaces de usuário interativas.
- [**vue-slick-carousel**](https://github.com/stasson/vue-slick-carousel) (^1.0.6) - Componente de carrossel para Vue.js, útil para exibir conteúdo de maneira atraente e funcional.

### **Ferramentas de Integração:**
- [**Langflow**](https://langflow.org/) - Ferramenta para orquestrar fluxos conversacionais, permitindo a construção de chatbots avançados com base no ChatGPT. Oferece uma interface de arrastar e soltar, facilitando o desenvolvimento de fluxos conversacionais complexos.
- [**DataStax Astra**](https://www.datastax.com/products/datastax-astra) - Banco de dados gerenciado baseado em Apache Cassandra, usado para armazenar e gerenciar dados de usuários, mensagens, e históricos de interação com o chatbot, garantindo escalabilidade e alta disponibilidade.

### **Ferramentas de Desenvolvimento:**
- [**@babel/core**](https://babeljs.io/) (^7.12.16) - Compilador JavaScript utilizado para garantir compatibilidade com várias versões de ECMAScript.
- [**@babel/eslint-parser**](https://github.com/babel/babel-eslint) (^7.12.16) - Parser que permite que o ESLint funcione com o código transpilado pelo Babel.
- [**@vue/cli-plugin-babel**](https://cli.vuejs.org/core-plugins/babel.html) (~5.0.0) - Plugin Babel para Vue CLI, utilizado para compilar e otimizar o código do projeto.
- [**@vue/cli-plugin-eslint**](https://cli.vuejs.org/core-plugins/eslint.html) (~5.0.0) - Plugin ESLint para Vue CLI, permitindo o linting do código.
- [**@vue/cli-service**](https://cli.vuejs.org/guide/cli-service.html) (~5.0.0) - Serviço CLI para Vue.js, responsável por automatizar tarefas de desenvolvimento.
- [**eslint**](https://eslint.org/) (^7.32.0) - Ferramenta de análise de código estático para identificar e corrigir problemas no código JavaScript.
- [**eslint-plugin-vue**](https://eslint.vuejs.org/) (^8.0.3) - Plugin para ESLint, focado nas melhores práticas para o desenvolvimento de componentes em Vue.js.

## Configuração do Projeto
Para configurar o projeto localmente, siga os passos abaixo:

### 1. Clonar o Repositório
Clone o repositório para o seu ambiente de desenvolvimento:
```bash
git clone https://github.com/SEU_USUARIO/petflow-chat-frontend.git
cd petflow-chat-frontend
```

### 2. Instalar Dependências
Instale todas as dependências necessárias para o funcionamento da aplicação:
```bash
npm install
# ou
yarn install
```

### 3. Executar a Aplicação
Inicie o servidor de desenvolvimento para rodar a aplicação localmente:
```bash
npm run serve
# ou
yarn serve
```
A aplicação estará disponível em [http://localhost:8080](http://localhost:8080).

## Estrutura de Diretórios

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
└── vue.config.js           # Configurações personalizadas do Vue CLI
```

## Contribuição
Contribuições são muito bem-vindas! Se você deseja contribuir com este projeto, siga os passos abaixo:

1. Faça um fork deste repositório.
2. Crie uma nova branch para sua feature (`git checkout -b feature/nome-da-sua-feature`).
3. Realize suas alterações e faça commit delas (`git commit -m 'Adicionando nova feature'`).
4. Envie suas alterações para o repositório remoto (`git push origin feature/nome-da-sua-feature`).
5. Abra um Pull Request e aguarde a análise.

---
