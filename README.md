# _studing-fastapi

Respositório com API de exemplo usando FastAPI no Python

## Descrição do projeto

Será um projeto de to-do list, onde será possível criar, listar, atualizar e deletar tarefas. O banco de dados utilizado será o PostgreSQL.

## Progresso

- [x] Criar _TO-DO_
- [x] Listar _TO-DOs_
- Atualizar _TO-DOs_
  - [ ] Renomear
  - [x] Marcar como completo/incompleto
- [ ] Apagar _TO-DO_

## Setup

### Gerenciador de dependências

Esse projeto de exemplo usa [Pipenv](https://pipenv.pypa.io/en/latest/) como gerenciador de dependências. Você precisa ter o Pipenv instalado na sua máquina para rodar o projeto.

Para instalar o Pipenv, você pode usar o comando:

```bash
pip install --user pipenv
```

> [!IMPORTANT]
> Para informações detalhadas sobre como instalar e usar o Pipenv, consulte a [documentação oficial](https://pipenv.pypa.io/en/latest/).

### Instalando as dependências

Para instalar as dependências do projeto, você pode usar o comando:

```bash
pipenv sync
```

Esse comando instala todas as dependências do projeto, incluindo as dependências de desenvolvimento, declaradas no arquivo [`Pipfile`](Pipfile).

### Rodando o projeto

Para rodar o projeto no modo desenvolvimento, você pode usar o comando:

```bash
pipenv run dev
```

Esse comando inicia o servidor de desenvolvimento do FastAPI. Você pode acessar a documentação da API em `http://localhost:8000/docs`.

## Estrutura do projeto

<!--
https://text.mateusf.com/text/tree?rootDot=true&trailingDirSlash=true&fullPath=false
```
.devcontainer
  devcontainer.json
  post-start.sh
app
  models/
    database.py
    dto.py
  routes/
  main.py
  database.py
.gitignore
Pipfile
Pipfile.lock
README.md
```
-->

```bash
.
├── .devcontainer/        # Configurações do DevContainer
│   ├── devcontainer.json # Configurações do DevContainer
│   └── post-start.sh     # Script de pós-start do DevContainer
├── app/                  # Código fonte da aplicação
│   ├── models/           # Modelos de dados
│   │   ├── database.py   # Modelos de entidades do banco de dados
│   │   └── dto.py        # Modelos de transferência de dados (Data-Transfer Objects)
│   ├── routes/           # Rotas da API
│   ├── main.py           # Arquivo principal da aplicação
│   └── database.py       # Configuração do banco de dados
├── .gitignore            # Arquivos e diretórios ignorados pelo Git
├── Pipfile               # Arquivo de definição de dependências e scripts
├── Pipfile.lock          # Arquivo de lock das dependências
└── README.md             # Documentação do projeto
```

## Links de referência

- **FastAPI**: [_https://fastapi.tiangolo.com/_](https://fastapi.tiangolo.com/)
- **Pipenv**: [_https://pipenv.pypa.io/en/latest/_](https://pipenv.pypa.io/en/latest/)
- **Pydantic**: [_https://docs.pydantic.dev/latest/_](https://docs.pydantic.dev/latest/)
