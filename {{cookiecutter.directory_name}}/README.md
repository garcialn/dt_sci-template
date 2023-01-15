# Apague esse arquivo README.md e utilize apenas o arquivo que vai ser gerado pelo github quando criar um repositório para seu projeto.
---

## Quick Start
---
### Set up do ambiente:
1. Instalar [Poetry](https://python-poetry.org/docs/#installation)
2. Preparar o ambiente virtual
```bash
make setup
make activate
```
### Instalar novas libs:
```bash
poetry add <package-name>
```
---
### Rodar script .py (processamento dos dados, treinamento, notebook):
```bash
make pipeline
```
---
### Rodar flow do Prefect
[flow](https://docs.prefect.io/concepts/flows/) é a base do Prefect (como todas as ferramentas de orquestração, como [Airflow](https://airflow.apache.org/) e [Metaflow](https://metaflow.org/)).

Para acompanhar flows pela UI do Prefect, basta criar uma conta no [Prefect Cloud](https://app.prefect.cloud/) ou rodar um servidor Prefect Orion no localhost.
```bash
prefect orion start
```
Abrir no browser http://127.0.0.1:4200/

![](images/prefect_cloud.png)
---
### Rodando flows pela UI

Depois de [fazer um deploy](https://towardsdatascience.com/build-a-full-stack-ml-application-with-pydantic-and-prefect-915f00fe0c62?sk=b1f8c5cb53a6a9d7f48d66fa778e9cf0), podemos rodar um flow pela UI com parâmetros padronizados:

![](https://miro.medium.com/max/1400/1*KPRQS3aeuYhL_Anv3-r9Ag.gif)
ou com parâmetros customizados:
![](https://miro.medium.com/max/1400/1*jGKmPR3aoXeIs3SEaHPhBg.gif)
---
### Gerar automaticamente documentação da API:

```bash
make docs_save
```
---
### Rodar os testes quando subir um PR (CI/CD):
![](images/github_actions.png)
