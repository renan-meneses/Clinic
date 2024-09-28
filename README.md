# Clinic

Este projeto é um **sistema de gerenciamento de atendimento para clínicas de saúde**. Ele foi desenvolvido com [Next.js](https://nextjs.org/) e [React](https://reactjs.org/), e inclui funcionalidades como agendamento de consultas, gerenciamento de pacientes, médicos e relatórios administrativos.

## Índice

- [Sobre o Projeto](#sobre-o-projeto)
- [Principais Funcionalidades](#principais-funcionalidades)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Pré-requisitos](#pré-requisitos)
- [Instalação](#instalação)
- [Como Usar](#como-usar)
- [Estrutura do Projeto](#estrutura-do-projeto)
- [Comandos Disponíveis](#comandos-disponíveis)
- [Contribuição](#contribuição)
- [Licença](#licença)

## Sobre o Projeto

O **Sistema de Atendimento de Clínica de Saúde** é uma solução completa para clínicas gerenciarem seus atendimentos médicos de maneira eficiente. O sistema permite que administradores e recepcionistas controlem agendamentos de consultas, mantenham o cadastro de médicos e pacientes, e acompanhem relatórios de produtividade e desempenho clínico.

Este sistema tem como objetivo otimizar o fluxo de trabalho, reduzir o tempo de espera de pacientes e garantir que o atendimento seja feito de forma organizada e eficaz.

## Principais Funcionalidades

- **Cadastro e gerenciamento de pacientes:** Informações pessoais, histórico médico, dados de contato.
- **Agendamento de consultas:** Marcação, visualização e controle de horários.
- **Gerenciamento de médicos:** Perfis médicos, especialidades, agenda de atendimentos.
- **Relatórios administrativos:** Relatórios de consultas, produtividade médica, entre outros.
- **Sistema de notificações:** Alertas para pacientes e médicos sobre consultas agendadas.

## Tecnologias Utilizadas

- **Next.js** - Framework React com renderização do lado do servidor (SSR).
- **React** - Biblioteca para construção de interfaces de usuário.
- **Node.js** - Plataforma para execução do JavaScript no servidor.
- **PostgreSQL** - Banco de dados relacional utilizado para armazenar informações de pacientes, médicos, consultas e relatórios.
- **TypeScript** - Superset de JavaScript para garantir maior segurança no código.
- **Yarn** ou **NPM** - Gerenciadores de pacotes.

## Pré-requisitos

Antes de rodar o projeto, você vai precisar ter os seguintes itens instalados:

- [Node.js](https://nodejs.org/en/) (versão 16 ou superior)
- [Yarn](https://yarnpkg.com/) ou [NPM](https://www.npmjs.com/)
- [PostgreSQL](https://www.postgresql.org/) para o banco de dados

Além disso, recomendamos um editor de código como [VSCode](https://code.visualstudio.com/).

## Instalação

Siga os passos abaixo para instalar e configurar o projeto localmente:

```bash
# Clone este repositório
git clone https://github.com/seu-usuario/sistema-clinica-saude.git

# Acesse a pasta do projeto
cd sistema-clinica-saude

# Instale as dependências
yarn install
# ou
npm install
```

### Configuração do Banco de Dados

Certifique-se de ter o PostgreSQL configurado e crie um banco de dados para o sistema:

1. Crie um banco de dados chamado `clinica_saude`.
2. Edite o arquivo `.env` na raiz do projeto com as credenciais de acesso ao banco de dados:

```
DB_HOST=localhost
DB_USER=seu-usuario
DB_PASSWORD=sua-senha
DB_NAME=clinica_saude
```

Após a configuração, rode as migrações do banco de dados:

```bash
# Execute as migrações para configurar as tabelas no banco de dados
yarn migrate
# ou
npm run migrate
```

## Como Usar

Para rodar a aplicação em modo de desenvolvimento:

```bash
# Inicie o servidor de desenvolvimento
yarn dev
# ou
npm run dev
```

Abra [http://localhost:3000](http://localhost:3000) no navegador para acessar a aplicação.

## Estrutura do Projeto

A estrutura de pastas do projeto é organizada da seguinte maneira:

```
.
├── pages                 # Páginas principais da aplicação
│   ├── api               # APIs internas da aplicação
│   └── index.tsx         # Página inicial de login
├── components            # Componentes reutilizáveis
├── styles                # Arquivos de estilos globais
├── services              # Serviços de comunicação com APIs e banco de dados
├── utils                 # Utilitários e helpers
├── migrations            # Arquivos de migração do banco de dados
├── public                # Arquivos públicos (imagens, ícones)
├── .env                  # Variáveis de ambiente
├── package.json          # Dependências e scripts do projeto
├── next.config.js        # Configurações do Next.js
└── README.md             # Documentação do projeto
```

## Comandos Disponíveis

Aqui estão alguns dos principais comandos disponíveis:

- **`yarn dev` ou `npm run dev`**: Executa a aplicação em modo de desenvolvimento.
- **`yarn build` ou `npm run build`**: Gera uma build otimizada para produção.
- **`yarn start` ou `npm run start`**: Inicia a aplicação em modo de produção.
- **`yarn migrate` ou `npm run migrate`**: Executa as migrações do banco de dados.
- **`yarn lint` ou `npm run lint`**: Verifica problemas no código utilizando o linter.

## Contribuição

Contribuições são sempre bem-vindas! Para contribuir:

1. Faça um fork deste repositório.
2. Crie uma nova branch para sua funcionalidade (`git checkout -b feature/nova-funcionalidade`).
3. Commit suas mudanças (`git commit -m 'Adiciona nova funcionalidade'`).
4. Faça o push para sua branch (`git push origin feature/nova-funcionalidade`).
5. Abra um Pull Request.

## Licença

Este projeto está licenciado sob a Licença **MIT**. Consulte o arquivo [LICENSE](./LICENSE) para mais detalhes.

---

Esse README fornece uma visão clara do projeto, com instruções sobre como configurá-lo, usá-lo e contribuir com ele. Ajuste conforme necessário para o seu caso específico.
