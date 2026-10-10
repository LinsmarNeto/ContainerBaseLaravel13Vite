# Container Docker Laravel 13.X + MySQL & PHP 8.5!

Este repositório fornece um ambiente Docker configurado para desenvolvimento com **Laravel 11**, **MySQL**, e **PHP 8.5**. A configuração foi projetada para simplificar o setup e oferecer uma base sólida para projetos modernos em Laravel.


# Recursos

-   **Laravel 13**: Framework PHP robusto e moderno para desenvolvimento web.
-   **PHP 8.5**: A versão mais recente do PHP com novos recursos e melhorias de desempenho.
-   **MySQL**: Banco de dados relacional para armazenamento de dados da aplicação.
-   **Vite**: Ferramenta de construção front-end extremamente rápida para aplicativos web.
-   **Docker Compose**: Configuração simplificada para gerenciar os serviços do ambiente.

## Estrutura

-   `docker-compose.yml`: Define os serviços Docker, incluindo os containers do PHP, MySQL e servidor web.
-   `Dockerfile`: Configura o ambiente PHP com as extensões necessárias para Laravel.
-   `html/`: Diretório onde o código do projeto Laravel será armazenado.

## Pré-requisitos

-   [Docker](https://www.docker.com/) instalado na sua máquina.
-   Docker Compose para gerenciamento de serviços.

## Como usar

 1. **Clone este repositório:**

    *git clone https://github.com/LinsmarNeto/ContainerBaseLaravel13Vite.git* 

    *cd ContainerBaseLaravel13Vite*

 2. **Entre na pasta ./html e crie o arquivo .env:**

    *cd html*

    *cp .env.example  .env*

 3. **Suba os containers:**

    *docker-compose up -d*

 4. **Acesse o container e instale as dependências do projeto:**

    *docker-compose  exec  app  bash*

    *composer  install*

 5. **Gere a key do projeto Laravel:**

    *php  artisan  key:generate*

 6. **Rodar as migrations:**

    *php  artisan  migrate*


 7. **Acesse o projeto:**

    *[http://localhost:8003](http://localhost:8003)*


Você é livre para usar, modificar e distribuir este repositório conforme suas necessidades!
Contribuições para melhorias também são bem-vindas. Aproveite o projeto!