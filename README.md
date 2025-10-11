# ML Project Scaffold

Este é um scaffold para projetos de Machine Learning, criado para fornecer uma estrutura inicial padronizada e robusta para novos projetos de ML. Ele utiliza o Cookiecutter para gerar um novo projeto com uma estrutura de diretórios predefinida, arquivos de configuração e exemplos de código.

## Organização do Projeto

A estrutura do projeto gerado é a seguinte:
```
    ├── LICENSE            <- Licença de código aberto, se escolhida
    ├── Makefile           <- Makefile com comandos de conveniência como `make data` ou `make train`
    ├── README.md          <- O README de nível superior para desenvolvedores que usam este projeto.
    ├── data
    │   ├── external       <- Dados de fontes de terceiros.
    │   ├── interim        <- Dados intermediários que foram transformados.
    │   ├── processed      <- Os conjuntos de dados canônicos e finais para modelagem.
    │   └── raw            <- O despejo de dados original e imutável.
    │
    ├── docs               <- Um projeto mkdocs padrão; consulte www.mkdocs.org para obter detalhes
    │
    ├── models             <- Modelos treinados e serializados, previsões de modelos ou resumos de modelos
    │
    ├── notebooks          <- Jupyter notebooks. A convenção de nomenclatura é um número (para ordenação),
    │                         as iniciais do criador e uma breve descrição delimitada por `-`, por exemplo,
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── pyproject.toml     <- Arquivo de configuração do projeto com metadados do pacote para
    │                         module_name e configuração para ferramentas como black
    │
    ├── references         <- Dicionários de dados, manuais e todos os outros materiais explicativos.
    │
    ├── reports            <- Análises geradas como HTML, PDF, LaTeX, etc.
    │   └── figures        <- Gráficos e figuras gerados para serem usados em relatórios
    │
    ├── requirements.txt   <- O arquivo de requisitos para reproduzir o ambiente de análise, por exemplo,
    │                         gerado com `pip freeze > requirements.txt`
    │
    ├── setup.cfg          <- Arquivo de configuração para flake8
    │
    └── module_name        <- Código-fonte para uso neste projeto.
        │
        ├── __init__.py    <- Torna module_name um módulo Python
        │
        ├── config.py      <- Armazena variáveis e configurações úteis
        │
        ├── dataset.py     <- Scripts para baixar ou gerar dados
        │
        ├── features.py    <- Código para criar recursos para modelagem
        │
        ├── modeling
        │   ├── __init__.py
        │   ├── predict.py <- Código para executar inferência de modelo com modelos treinados
        │   └── train.py   <- Código para treinar modelos
        │
        └── plots.py       <- Código para criar visualizações
```

Create Scaffold Repository (create_repo.yml): 

Este workflow permite que você gere um novo repositório a partir do scaffold preenchendo as variáveis do Cookiecutter por meio de inputs do workflow.