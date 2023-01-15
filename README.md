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
│   ├── final                       # Dados após treino do modelo
│   ├── processed                   # Dados processados (em caso de uso local)
│   ├── raw                         # Dados brutos (em caso de uso local)
├── docs                            # Documentação do projeto
├── .flake8                         # Configuração para formatação flake8
├── .gitignore                      # Arquivos/Diretórios a serem ignorados pelo git
├── Makefile                        # Arquivos das rotinas criadas para usar no terminal
├── models                          # Modelos do projeto
├── notebooks                       # Notebooks do projeto
├── .pre-commit-config.yaml         # Configurações pré-commit
├── pyproject.toml                  # Dependencias do Poetry
├── README.md                       # Descrição do Projeto
├── src                             # Código fonte do projeto
│   ├── __init__.py                 # Transformar o diretório em Módulo Python
│   ├── config.py                   # Configurações do código
│   ├── process.py                  # Código de processamento dos dados para treinamento do(s) modelo(s)
│   ├── run_notebook.py             # Rodar notebook
│   └── train_model.py              # Modelo para treinamento
└── tests                           # Diretório de testes
    ├── __init__.py                 # Transformar o diretório em Módulo Python
    ├── test_process.py             # Funções para teste de process.py
    └── test_train_model.py         # Funções para teste de train_model.py
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
