# Data4All - ML Project

- Instituição: Let's Code
- Curso: Data4All
- Disciplina: Machine Learning I
- Professores: Braian Bispo, Renato Marques & Thiago Kuma
- Alunos: Aline Cristina De Carvalho Estanislau, André Alves Teixeira, Eduardo Vitor G Silva, Felipe Cunha & Matheus Miranda Brandão.

Este projeto é uma exploração do dataset: [Employee Attrition](https://aiplanet.com/challenges/177/data-sprint-56-employee-attrition-177/data), fornecido pelo [AI Planet](https://aiplanet.com/). O foco é explorar os dados e descobrir quaisquer insights interessantes ou padrões que possam estar presentes, afim de decidir e implementar um modelo de Machine Learning.

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
> Metadados extraídos do site oficial do [AI Planet](https://aiplanet.com/).

Este dataset apresenta um questionário envolvendo funcionários da IBM, indicando se existe uma rotatividade ou não. Os dados possuem aproximadamente 1200 entradas.
- Id
- Age - Idade do funcionário
- Attrition - Rotatividade
    - 0 'No'
    - 1 'Yes'
- BusinessTravel - Frequência de viagem do funcionário
- Department - Departmento de trabalho
- DistanceFromHome - Distância da casa do funcionário até o trabalho
- EducationField - Área de estudo do funcionário
- EmployeeNumber - Número de identificação do funcionário
- EnvironmentSatisfaction - Satisfação com o ambiente de trabalho
- Gender - Gênero do funcionário
- MartialStatus - Estado civil do funcionário
- MonthlyIncome - Salário mensal do funcionário
- NumCompaniesWorked - Número de empresas que o funcionário já trabalhou anteriormente
- OverTime - Se o funcionário trabalha horas extras ou não
- PercentSalaryHike - Porcentagem de aumento salarial
- StockOptionLevel - Nível de opções de ações
- TotalWorkingYears - Total de anos trabalhados
- TrainingTimesLastYear - Número de treinamentos realizados no último ano
- YearsAtCompany - Número de anos trabalhados na empresa
- YearsInCurrentRole - Número de anos no cargo atual
- YearsSinceLastPromotion - Número de anos desde a última promoção
- YearsWithCurrManager - Número de anos com o atual gerente
- Education
    - 1 'Below College'
    - 2 'College'
    - 3 'Bachelor'
    - 4 'Master'
    - 5 'Doctor'
- EnvironmentSatisfaction
    - 1 'Low'
    - 2 'Medium'
    - 3 'High'
    - 4 'Very High'
- JobInvolvement
    - 1 'Low'
    - 2 'Medium'
    - 3 'High'
    - 4 'Very High'
- JobSatisfaction
    - 1 'Low'
    - 2 'Medium'
    - 3 'High'
    - 4 'Very High'
- PerformanceRating
    - 1 'Low'
    - 2 'Good'
    - 3 'Excellent'
    - 4 'Outstanding'
- Behaviour
    - 1 'Good'
    - 2 'Bad'
    - 3 'Not Rated'
- CommunicationSkill
    - 1 'Bad'
    - 2 'Average'
    - 3 'Good'
    - 4 'Better'
    - 5 'Best'
- StockOptionLevel
    - 0 'No stocks'
    - 1 'Less Stocks'
    - 2 'Moderate Stocks'
    - 3 'A lot of Stocks'

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

- NumPy;
- Pandas;
- Matplotlib;
- Seaborn;
- Scikit-learn;
- ipykernel.

# Integrantes

- [Aline Cristina De Carvalho Estanislau](https://github.com/alinecarvalhoz)
- [André Alves Teixeira](https://github.com/decoteixeira)
- [Eduardo Vitor G Silva](https://github.com/edulopo)
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
│   │   └── raw
│   │   │   ├── testing_data.csv
│   │       └── training_data.csv
│   ├── notebooks
│   │   ├── model.ipynb
│   │   └── eda
│   │       └── matheus.ipynb
│   └── outputs
│       └── ...
└── utils
    ├── environment.yml
    └── requirements.txt
```

# Contribuições
...