# Data4All - ML Project

- Instituição: Let's Code
- Curso: Data4All
- Disciplina: Machine Learning I
- Professores: Braian Bispo, Renato Marques & Thiago Kuma
- Alunos: Aline Cristina De Carvalho Estanislau, André Alves Teixeira, Eduardo Vitor G Silva, Felipe Cunha & Matheus Miranda Brandão.

Este projeto é uma exploração do dataset: [Dataset](...), fornecido pelo [Kaggle](https://www.kaggle.com/). O foco é explorar os dados e descobrir quaisquer insights interessantes ou padrões que possam estar presentes, afim de decidir e implementar um modelo de Machine Learning.

A especificação completa do projeto pode ser encontrada em: [Projeto Final](https://github.com/MatBrands/Data4All_ML_Project).

## Conteúdo

- Descrição dos Dados
- Objetivos
- Ferramentas Usadas
- Integrantes
- Recomendações
- Instalação
- Organização do projeto
- Contribuições

# Descrição dos Dados


# Objetivos

Os objetivos deste projeto são: 

- Demonstrar as habilidades obtidas em aula;
- Simular a resolução de um problema real;
- Descobrir padrões e relações entre as variáveis;
- Entender melhor os conceitos de Machine Learning;
- Construir e aplicar um modelo de Machine Learning;
- Interpretar os resultados obtidos.
# Ferramentas Usadas
Este projeto foi concluído usando Python e suas bibliotecas associadas, como:

- NumPy,
- Pandas,
- Matplotlib,
- Seaborn,
- Scikit-learn,
- ipykernel.

# Integrantes

- [Aline Cristina De Carvalho Estanislau](https://github.com/alinecarvalhoz)
- [André Alves Teixeira]()
- [Eduardo Vitor G Silva](https://github.com/decoteixeira)
- [Felipe Cunha](https://github.com/felpscunha)
- [Matheus Miranda Brandão](https://github.com/MatBrands/)

# Recomendações
Neste projeto foi adotado o uso de Commits Semânticos para padronização:

- Feat: Nova feature do projeto
- Refactor: Refatoração de alguma parte do código
- Fix: Correção de erros que estão causando bugs
- Chore: Mudanças que não influenciam o sistema nem arquivos de testes
- Style: Mudanças de formatação ou estilos de códigos que não influenciam na lógica do sistema
- Test: Criação ou alteração de algum código de teste
- Perf: Alterações feitas para melhorar a performance do projeto
- Docs: Alterações na documentação do projeto

# Instalação

## Instalação
Foi utilizado o [Python](https://www.python.org/) v3.11.

### Conda
No desenvolvimento foi utilizado o gerenciador de pacotes e ambientes [Conda](https://conda.io/). Portanto para prosseguir necessita-se de sua [instalação](https://conda.io/projects/conda/en/latest/user-guide/install/index.html).

- Navegar até a pasta de destino
```sh
cd utils
```

- Instalar dependências
```sh
conda env create -f environment.yml
```

- Ativar
```sh
conda activate ada_ml_venv
```

- Desativar
```sh
conda deactivate
```

### Requirements
Pode-se utilizar o arquivo requirements.txt para criar o ambiente virtual.

- Criar ambiente virtual
```sh
python -m venv ada_ml_venv
```

- Ativar
```sh
source ./ada_ml_venv/bin/activate
```

- Navegar até a pasta de destino
```sh
cd utils
```

- Instalar dependências
```sh
pip install -r requirements.txt
```

- Desativar
```sh
deactivate
```

# Organização do projeto

```sh
.
├── License
├── Readme.md
├── main
│   ├── datasets
│   │   └── ...
│   ├── models
│   │   └── ...
│   ├── notebooks
│   │   └── ...
│   └── raw
│       └── ...
└── utils
    ├── environment.yml
    └── requirements.txt
```

# Contribuições
...