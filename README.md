# Teste Backend

Leia primeiro todo o projeto, faça sua estimativa de horas para o desenvolvimento e envie um email com o
título `[Teste Backend] Estimativa` para rh@nanoincub.com.br

Quando finalizar o teste, publique tudo no seu [Github](https://github.com) e envie um email com o
título `[Teste Backend] Finalizado` para rh@nanoincub.com.br contendo o link do repositório do projeto

## Atenção:

Coloque no `README.md` do seu projeto todas as instruções para conseguirmos executá-lo. Se possivel, informe a versão do PHP, versão do mysql

Se estiver utilizando docker ou vagrant, coloque os arquivos junto ao projeto para que possamos rodar o ambiente de desenvolvimento.


## Missão

- Desenvolver um **Painel Administrativo** em **PHP** para gestão de Produto e Estoque
- Lembre-se, este é um teste de contratação, você estará vendendo um produto chamado você, portanto, esperamos um projeto com máximo de qualidade que você consegue entregar.


## O que será avaliado

- Iremos avaliar TUDO, exatamente TUDO: técnica, arquitetura, conhecimento de Banco de Dados, qualidade de layout, segurança, esforço, criatividade, etc.


## Requisito mínimo do projeto

- Funcionar, portanto, tome cuidado ao subir no git, verifique se o projeto que você subiu no git está funcionando.


### Especificação

Monte uma base de produto com a seguinte estrutura:

Produto:
```
nome:               string
preco:              string
quantidade_estoque: int ## O valor deve ser: Total de entradas do produto - Total de saídas do produto
categoria_id:       int
data_criacao:       datetime
data_alteracao:     datetime
```

Categoria de produto:
```
nome:               string
data_criacao:       datetime
data_alteracao:     datetime
```

Registro:
```
nota_fiscal:        string
referencia:         string
produto_id:         int
quantidade:         int
tipo:               (escolha o tipo que se encaixa melhor para esta coluna, é com essa coluna que você irá informar se é um registro de entrada ou saída)
id_usuario_logado   int
data_criacao:       datetime
data_alteracao:     datetime
```

Utilize **MySQL** para armazenar os dados.

### Funcionalidades da Aplicação

- `Login`

Página de Login com campo usuário e senha.

---

`Listagem de Produto`

Listagem dos produtos exibindo o ID, Nome,Categoria, Preco e Quantidade de Estoque. A listagem deverá ter paginação.

---

`Cadastro de Produto`

Formulário de cadastro com os campos do produto

---

`Edição de Produto`

Formulário de edição com os campos do produto

---

`Excluir Produto`

Um botão de deletar na listagem de produtos onde o usuário poderá excluir o produto cadastrado.

---

`Filtro de Pesquisa na Listagem de Produto`

A Listagem de Produto deverá conter um filtro por **Nome do Produto** e pela **Categoria**.

---

`Listagem de Categoria de Produto`

Listagem das categorias do produtos apenas com paginação.

---

`Cadastro de Categoria de Produto`

Formulário de cadastro com os campos da categoria do produto

---

`Edição de Categoria de Produto`

Formulário de edição com os campos da categoria do produto

---

`Excluir  Categoria de Produto`

Um botão de deletar na listagem de categorias de produtos onde o usuário poderá excluir a categoria cadastrada.

---

`Listagem de entrada e saida`

Listagem de entrada e saída dos produtos exibindo o ID, Nome do produto, Categoria, Tipo(Entrada ou saída), Quantidade e Usuário que lancou o registro. A listagem deverá ter paginação.

---

`Cadastro de Entrada`

Formulário de cadastro de entrada, deverá informa o produto, a nota fiscal e a quantidade.

---

`Cadastro de Saída`

Formulário de cadastro de saida deverá informar o produto, o código de referencia e a quantidade.


---

## Sugestões
Você pode utilizar algum framework para auxiliar no desenvolvimento da interface, por exemplo:

[https://getbootstrap.com/docs/3.3/css/](https://getbootstrap.com/docs/3.3/css/)

[https://adminlte.io/themes/AdminLTE/index2.html](https://adminlte.io/themes/AdminLTE/index2.html)

[https://startbootstrap.com/template-overviews/sb-admin-2/](https://startbootstrap.com/template-overviews/sb-admin-2/)


### Framework PHP desejado
[CodeIgniter 3.x](https://github.com/bcit-ci/CodeIgniter) (*Opcional*)

ou

[Laravel 5.7+](https://github.com/laravel/laravel) (*Opcional*)


## Dúvida

Se tiver qualquer dúvida sobre esse teste, envie um email com o título `[Teste Backend] O assunto da dúvida` para rh@nanoincub.com.br
