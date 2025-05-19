# Marcação de Presença com Reconhecimento Facial

Este projeto é uma aplicação simplificada de marcação de presença utilizando reconhecimento facial, desenvolvida para fins didáticos e como estudo de caso em um livro. A aplicação é dividida em duas partes principais: o front-end e o back-end.

## Estrutura do Projeto

-   **Raiz do Projeto:** Contém os arquivos do front-end.
-   `backend/app/`: Contém os arquivos do back-end.

## Front-end

O front-end é implementado como uma Single Page Application (SPA) utilizando HTML, CSS e JavaScript puro. Ele é responsável por:

-   Captura de imagens da câmera.
-   Extração de características faciais utilizando a biblioteca face-api.js.
-   Comunicação com o back-end através de requisições HTTP (API REST).
-   Exibição da interface do usuário.

**Observação:** Nesta versão simplificada, a validação facial é realizada no front-end. Em uma versão mais robusta, essa validação seria movida para o back-end para maior segurança e confiabilidade.

## Back-end

O back-end é desenvolvido em PHP e utiliza um banco de dados MySQL. Ele é responsável por:

-   Receber requisições do front-end (API REST).
-   Armazenar e consultar dados de usuários e presenças no banco de dados.
-   Retornar respostas em formato JSON para o front-end.

### Roteamento Simplificado

Para fins didáticos, o roteamento do back-end foi simplificado. Em um cenário real, seria recomendado o uso de um framework PHP como Laravel ou Symfony para um roteamento mais robusto e organizado.

### Instalação do Composer

1.  Navegue até o diretório `backend/` no terminal:

    ```sh
    cd backend
    ```
2.  Execute o comando para instalar as dependências do projeto:

    ```sh
    composer install
    ```

### Script do Banco de Dados

O script para criação do banco de dados está localizado em `backend/app/database`. Importe este script para o seu servidor MySQL para criar as tabelas necessárias para a aplicação.

### Executar
Tenha certeza que o PHP está instalado corretamente no sistema operacional e apontado corretamente nas variáveis de ambiente, e o banco MySQL esteja instalado e com as tabelas e banco criados.
na pasta do projeto na raiz execute o comando:
```
php -S localhost:8080

```