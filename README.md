
# 🔒 Projeto Autenticação/Autorização com JSON Web Token 
Projeto de uma SPA (Single Page Application) Angular que consome uma API de ASP.NET para cadastrar, logar, autenticar e autorizar usuários através do ASP.NET Identity juntamente com SQL Server. A seção de cadastro de usuários envia um código de autenticação no email do usuário para completar o cadastro. Dentro da home, o usuário pode adicionar a permissão de Admnistrador para acessar endpoints que ficam ocultos/não autorizados até que ele ganhe permissão para isso. Toda a dinâmica de autenticação e autorização foi realizada pela da manipulação do Session Storage do browser.




## 🌐 Stack Utilizada

**Front-end:** Angular - TypeScript - HTML - SCSS - Bootstrap - PrimeNG

**Back-end:** C# - API de ASP.NET - Entity Framework Core - ASP.NET Identity 

**Banco de Dados:** SQL Server


## 🧠 Conhecimentos Utlizados/Adquiridos

- Angular
- Componentes 
- PrimeNG
- Consumo de API através da HttpClient
- ASP.NET Identity
- Autenticação/Autorização com JWT (JSON Web Token)
- Composição de um Token JWT 
- View Models 

- É necessário ter o .NET 7.0 instalado ➡️ https://dotnet.microsoft.com/pt-br/download/dotnet/7.0
- É necessário ter o Node instalado ➡️ https://nodejs.org/en/download/current
- É necessário o uso de SQL Server para o banco de dados https://www.microsoft.com/pt-br/sql-server/sql-server-downloads
- Recomendo o uso do Visual Studio Code para rodar a aplicação


Clone o projeto

```bash
  git clone https://github.com/vini-fumagalli/app-desktop-controle-gastos.git
```

Vá até o diretório do projeto

```bash
  cd app-desktop-controle-gastos
```

Clone os submódulos do back-end e front-end do projeto 

```bash
  git submodule init
  git submodule update

```

Crie a variável de ambiente `DB_CONNECTION_GASTOS`

```
Data Source=localhost/SQLEXPRESS;Initial Catalog=DB_ControleGastos;Trusted_Connection=True;TrustServerCertificate=true;
```

Navegue até a pasta src do back-end e aplique as migrações para o Banco de Dados

```bash
  cd back-end-controle-gastos/src
  dotnet ef migrations add FirstMigration
  dotnet ef database update 
```

Inicie a aplicação

`pressione (F5)`

Navegue até a pasta do front-end, instale o Electron e inicie a aplicação

```bash
  cd front-end-controle-gastos
  npm install electron --save-dev
  npm start
```


    
## 🙋 Autor

- Vinícius Fumagalli
- Estagiário de back-end com .NET
- Cursando 5º período de Ciência da Computação


## 🔗 Meus Links
[![portfolio](https://img.shields.io/badge/portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://github.com/vini-fumagalli)

[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/vin%C3%ADcius-fumagalli-b59313250/)
