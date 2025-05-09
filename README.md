# Plataforma de Estudos Interativa
## Descrição
Este projeto é uma plataforma de estudos interativa onde os usuários podem criar flashcards, organizá-los por categoria e dificuldade, e iniciar desafios para testar seus conhecimentos. A plataforma também fornece insights de desempenho por meio de gráficos detalhados, permitindo que os usuários acompanhem efetivamente seu progresso de aprendizado.

## Tecnologias Utilizadas
Este projeto foi desenvolvido utilizando **Python** com o framework **Django**. Também houve um trabalho significativo com HTML, CSS e JavaScript para estruturar as páginas, mas a principal linguagem utilizada é Python.

## Recomendações 
- Ter o <a href="https://code.visualstudio.com">Visual Studio Code</a> instalado.  
- Utilizar a extensão *SQLite Viewer* para melhor visualização do banco de dados.
- Rodar o código dentro do ambiente virtual.

## Executando o Projeto
Para rodar o projeto, é recomendável usar um **ambiente virtual**. Siga estes passos:

Ative o ambiente virtual com o comando: `.\venv\Scripts\Activate`
Execute o servidor com o comando: `python manage.py runserver`

Clique no link que aparecerá no terminal para abrir a página no localhost:

<p align="center">
<img src="https://github.com/LeRodrigues2005/StudyAsync/assets/97632543/f8007554-9e28-472c-8f2c-ff01dd8d041d" alt="" width="600">
</p>

## Banco de Dados
O projeto utiliza o banco de dados **db.sqlite3**. Alguns nomes de usuários e senhas foram pré-criados para fins de teste e estão salvos no banco de dados.

## Funcionalidades e Detalhes
Abaixo estão os passos e funcionalidades da plataforma, cada um acompanhado por imagens para melhor compreensão:

### 1. **Iniciando a Aplicação:**
Após rodar o servidor e clicar no link no terminal, a página será aberta no localhost, iniciando com a seguinte interface:
<p align="center">
<img src="https://github.com/LeRodrigues2005/StudyAsync/assets/97632543/e4fc34d3-5d08-4d37-aaeb-d937cd2fc717" alt="" width="900">
</p>

### 2. **Cadastro de Usuário:**
Crie um novo nome de usuário e senha para se registrar.

*Obs: Se o nome de usuário já estiver registrado, você será redirecionado para a página de login.*

<p align="center">
<img src="https://github.com/LeRodrigues2005/StudyAsync/assets/97632543/8a70b7c6-3d9c-4d98-9bcd-9a20e7471644" alt="" width="500">
</p>

### 3. **Segurança das Senhas:**
As senhas são armazenadas no banco de dados e protegidas usando PBKDF2 (Password-Based Key Derivation Function 2) com o algoritmo de hash SHA-256.

<p align="center">
<img src="https://github.com/LeRodrigues2005/StudyAsync/assets/97632543/d44a1c56-f527-4647-91e0-0c28f32590e3" alt="" width="400">
</p>


### 4. **Acesso à Página Inicial:**
Após fazer o login, você terá acesso à página inicial da plataforma.

<p align="center">
<img src="https://github.com/LeRodrigues2005/StudyAsync/assets/97632543/cc81a4a2-b4c9-4efd-9a5d-7af053d088d6" alt="" width="900">
</p>

### 5. **Opções de Flashcard:**
Clicando na opção *Flashcard* no menu, você pode escolher entre várias opções, sendo *Criar Flashcard* a página inicial.
<p align="center">
<img src="https://github.com/LeRodrigues2005/StudyAsync/assets/97632543/3a960ff4-8642-4e67-8d4e-578656d92168" alt="" width="400">
</p>

### 6. **Criando Flashcards:**
Na página inicial da plataforma (Criar Flashcard), você pode criar seus próprios flashcards, escolhendo entre três categorias disponíveis (Português, Matemática e Programação) e três níveis de dificuldade (Fácil, Médio, Difícil). Basta criar a pergunta, digitar a resposta, categorizar e clicar em *enviar*. O flashcard criado aparecerá ao lado do container. 
<p align="center">
<img src="https://github.com/LeRodrigues2005/StudyAsync/assets/97632543/2a051299-252e-4e75-bfe6-4ed395b32c8c" alt="" width="900">
</p>

*Obs: Você pode filtrar seus flashcards para visualizar melhor o que já criou.*
<p align="center">
<img src="https://github.com/LeRodrigues2005/StudyAsync/assets/97632543/9f511bfd-df27-4314-9ca8-43c0dca0ebd7" alt="" width="500">
</p>

### 7. **Iniciando um Desafio:**
Clicando na opção "Iniciar Desafio", você poderá escolher uma categoria, dificuldade e quantidade de questões, conforme os flashcards que você já criou.

<p align="center">
<img src="https://github.com/LeRodrigues2005/StudyAsync/assets/97632543/7c8fd202-d861-49f0-b24e-e81772d81e7e" alt="" width="900">
</p>

*Obs: Se você criou, por exemplo, 5 flashcards de matemática na dificuldade média e iniciar um desafio de 6 flashcards de matemática da dificuldade média, não irá carregar e você terá que digitar de novo.*

### 8. **Página do Desafio:**
Após iniciar um desafio, você será redirecionado para a página do desafio com o status *em aberto* até que seja respondido. Você pode acessar o desafio clicando na ID dele (o número na coluna *desafio*).

<p align="center">
<img src="https://github.com/LeRodrigues2005/StudyAsync/assets/97632543/22c96c8c-e7be-40bb-ae7f-e4cd3fb1ce25" alt="" width="900">
</p>

### 9. **Respondendo ao Desafio:**
Você pode responder mentalmente às perguntas dos flashcards e marcar se acertou ou não (na parte inferior do flashcard). Você consegue ver a resposta clicando na pergunta.

<p align="center">
<img src="https://github.com/LeRodrigues2005/StudyAsync/assets/97632543/0283e3e4-d41f-4966-bd18-058fe80403f6" alt="" width="900">
</p>


### 10. **Relatório do Desafio:**
Após responder, as perguntas ficam mais escuras e você pode analisar o gráfico conforme a quantidade de erros e acertos clicando em *Relatório Detalhado*.

<p align="center">
<img src="https://github.com/LeRodrigues2005/StudyAsync/assets/97632543/3e66a684-e162-46f4-b24b-57474ba7e5fe" alt="" width="900">
</p>

<p align="center">
<img src="https://github.com/LeRodrigues2005/StudyAsync/assets/97632543/50f5ac77-c044-46ae-b488-94142c64fb90" alt="" width="900">
</p>


### 11. **Apostilas:**
Clicando na opção *Apostilas* no cabeçalho da página, você será redirecionado para uma página onde é possível ver as apostilas existentes em sua conta ou adicionar novas. Quando uma apostila for adicionada, você poderá clicar em *Abrir* para visualizar a apostila clicando em sua capa (espere alguns segundos para a apostila carregar).

<p align="center">
<img src="https://github.com/LeRodrigues2005/StudyAsync/assets/97632543/c6332ba8-ca6c-49b1-9353-72466e4ee9f8" alt="" width="400">
</p>

<p align="center">
<img src="https://github.com/LeRodrigues2005/StudyAsync/assets/97632543/fdb2efae-02e0-4d42-9604-60f8849d593d" alt="" width="900">
</p>


### 12. **Visualizações de Apostilas:**
Cada vez que a apostila for visualizada, o contador *views totais* é atualizado.

### Informações Adicionais
Sinta-se à vontade para explorar e contribuir com este projeto. Seu feedback e sugestões são altamente apreciados.
