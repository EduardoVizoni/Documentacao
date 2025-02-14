# Sistema de Gerenciamento de Biblioteca

## Índice
- [Sobre o Projeto](#sobre-o-projeto)
- [Recursos](#recursos)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Como Executar o Projeto](#como-executar-o-projeto)
- [Pré-requisitos](#pré-requisitos)
- [Passo a Passo](#como-executar)
- [Documentação da API](#documentação-da-api)
- [Contribuindo](#contribuindo)
- [Licença](#licença)
- [Contato](#contato)

---

## Sobre o Projeto
O **Sistema de Gerenciamento de Biblioteca** foi desenvolvido para facilitar o processo de empréstimo, devolução e gerenciamento de livros em uma biblioteca. Através da aplicação, é possível gerenciar empréstimos de livros, disponibilidade de exemplares, cadastro de usuários e gerar relatórios de atividades. O sistema visa melhorar a experiência do usuário e otimizar a administração da biblioteca, garantindo uma gestão eficiente e eficaz.

---

## Recursos

- **Cadastro e gerenciamento de livros**: Informações detalhadas como título, autor, ISBN, etc.
- **Criação e modificação de empréstimos**: Opções de data de empréstimo e devolução.
- **Visualização da disponibilidade dos livros**: Consulta em tempo real.
- **Geração de relatórios**: Empréstimos, devoluções e multas.
- **Notificação de usuários**: Alertas sobre empréstimos e devoluções.
- **Sistema de login e autenticação**: Para administradores e usuários.

---

## Tecnologias Utilizadas

### Frontend
- ![Angular](https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white)  
  **Angular**: Framework utilizado para o desenvolvimento da interface de usuário, permitindo uma aplicação interativa e responsiva.

### Backend
- ![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white)  
  **Spring Boot (Java)**: Framework utilizado para o desenvolvimento da API, que gerencia os empréstimos, os livros e os usuários.

### Banco de Dados
- ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)  
  **MySQL**: Banco de dados relacional utilizado para armazenar informações sobre empréstimos, usuários e livros.

### Autenticação
- ![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=json-web-tokens&logoColor=white)  
  **JWT (JSON Web Tokens)**: Utilizado para garantir a segurança no processo de autenticação e autorização de usuários.

---

# Como Executar o Projeto

### Pré-requisitos
Certifique-se de ter os seguintes itens instalados:

- ![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)  
  **Node.js**: Para o frontend Angular.

- ![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)  
  **Java JDK**: Para o backend Spring Boot.

- ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)  
  **MySQL**: Para o banco de dados.

### Como Executar

### Passo 1: Clone o Repositório
Clone o repositório para o seu ambiente local com o comando:

```bash
git clone https://github.com/usuario/sistema-biblioteca.git
```

### Passo 2: Instale as Dependências do Frontend
Navegue até o diretório do frontend e instale as dependências com npm:

```bash
cd sistema-biblioteca/frontend
npm install
```

### Passo 3: Instale as Dependências do Backend
Navegue até o diretório do backend e instale as dependências com Maven:

```bash
cd sistema-biblioteca/backend
mvn install
```
### Passo 4: Configuração do Banco de Dados
Crie um banco de dados MySQL e configure as credenciais no arquivo application.properties do backend. Em seguida, execute as migrações para criar as tabelas necessárias:

```bash
spring.datasource.url=jdbc:mysql://localhost:3306/biblioteca
spring.datasource.username=seu_usuario
spring.datasource.password=sua_senha
```

### Passo 5: Inicie o Servidor Backend
Inicie o servidor do backend com o comando:

```bash
mvn spring-boot:run
```

### Passo 6: Inicie o Servidor Frontend
Inicie o servidor do frontend com o comando:

```bash
ng serve
```

### Passo 7: Acesse a Aplicação
Abra o navegador e acesse a aplicação na URL: http://localhost:4200.

---

## Documentação da API
A API do Sistema de Gerenciamento de Biblioteca foi documentadautilizando **Swagger**, permitindo uma visualização interativa e detalhada de todos os endpoints disponíveis. Abaixo estão alguns dos endpoints principais:
- **GET /api/books:** Retorna todos os livros disponíveis.
- **POST /api/loans:** Cria um novo empréstimo de livro.
- **GET /api/loans/{id}:** Obtém os detalhes de um empréstimo específico.
- **PUT /api/loans/{id}:** Atualiza informações de um empréstimo.
- **DELETE /api/loans/{id}:** Cancela um empréstimo.

Para acessar a documentação completa da API no Swagger, inicie o servidor backend e acesse:
```bash
http://localhost:8080/swagger-ui.html
```

---

## Contribuindo
**1.** Faça um fork do repositório.  
**2.** Crie uma nova branch (`git checkout -b feature-nome-da-feature`).  
**3.** Faça as alterações e commit (`git commit -am 'Adiciona nova feature'`).  
**4.** Envie para o repositório original (`git push origin feature-nome-da-feature`).  
**5.** Abra um pull request descrevendo as mudanças feitas.

## Licença

Este projeto está licenciado sob a **Licença MIT** - veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

## Contato

Se você tiver alguma dúvida ou sugestão, entre em contato com a equipe de desenvolvimento:

- **Email**: vizoni.prado@gmail.com  
- **Telefone**: +55 55 5555-5555 
