[![View on Medium](https://img.shields.io/badge/Medium-View%20on%20Medium-blue?logo=medium)](https://pydt.medium.com/come%C3%A7ando-seu-projeto-de-data-science-f2c99ff0becc)

# Ciência de Dados Cookie Cutter

Repositório com estrutura padrão para projetos de Ciência de Dados. O template original foi desenvolvido pela Cientista de Dados Khuyen Tran, que frequentemente compartilha artigos muito interessantes e úteis para Análise e Ciência de Dados de todas as senioridades.

[![View on Medium](https://img.shields.io/badge/Medium-View%20on%20Medium-blue?logo=medium)](https://khuyentran1476.medium.com/)

---

## Tools used in this project
* [Poetry](https://python-poetry.org/docs/master/#installing-with-the-official-installer): Gerenciamento de dependências e pacotes 
* [DVC](https://dvc.org/): Versionamento de Dados
* [Pydantic](https://docs.pydantic.dev/): Validação de dados
* [Plugins pré-commit](https://pre-commit.com/): Automação de formatação do código pré-commit
* [Makefile](https://the-turing-way.netlify.app/reproducible-research/make/make-examples.html): Criação de funções para rotinas de comando no terminal
* [GitHub Actions](https://docs.github.com/en/actions): Automação de fluxo para build, teste e deploy de código (CI/CD)
* [pdoc](https://github.com/pdoc3/pdoc): Automação de criação de documentação para API do projeto
## Estrutura de Projetos
```bash
.
├── data            
│   ├── final                       # data after training the model
│   ├── processed                   # data after processing
│   ├── raw                         # raw data
├── docs                            # documentation for your project
├── .flake8                         # configuration for flake8 - a Python formatter tool
├── .gitignore                      # ignore files that cannot commit to Git
├── Makefile                        # store useful commands to set up the environment
├── models                          # store models
├── notebooks                       # store notebooks
├── .pre-commit-config.yaml         # configurations for pre-commit
├── pyproject.toml                  # dependencies for poetry
├── README.md                       # describe your project
├── src                             # store source code
│   ├── __init__.py                 # make src a Python module
│   ├── config.py                   # store configs 
│   ├── process.py                  # process data before training model
│   ├── run_notebook.py             # run notebook
│   └── train_model.py              # train model
└── tests                           # store tests
    ├── __init__.py                 # make tests a Python module 
    ├── test_process.py             # test functions for process.py
    └── test_train_model.py         # test functions for train_model.py
```
---

## Como usar o template

Instalar Cookiecutter:
```bash
pip install cookiecutter
```

Criando um projeto:
```bash
cookiecutter https://github.com/garcialn/dt_sci-template
```
