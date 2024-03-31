# Projeto-01-AI900
## Trabalhando com Machine Learning na Prática no Azure ML
## Objetivo
### Utilize a ferramenta Azure Machine Learning Microsoft para criar, treinar e testar um modelo de aprendizado para o aluguel de bicicletas utilizando os dados disponíveis para teste.


Passo a passo está na documentação oficial da Microsoft: [aqui](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/01-machine-learning.html)

1. Criar nosso Workspace 
2. Iniciar novo trabalho de ML automatizado. 
    * Nome do trabalho: msleam-bike-automl
    * Tipo de tarefa **regressão**
    * Nome do ativo de dados: Aluguel de bicicleta.
    * Tipo ativo de dados Tabular.
    * Fonte de dados: De um arquivo da Web.
    *seguir configuração da documentação 
    * **os nomes e fonte de dados, usei exatamente o da documentação**


3. Enviar trabalho(Aguarde configuração)
4. Finalizado, é hora de validar nossas métricas.
5. Criar Modelo para testar ponto de extremidade.

## Teste
```
{
  "input_data": {
    "data": [
       {
         "day": 10,
         "mnth": 5,   
         "year": 2023,
         "season": 1,
         "holiday": 0,
         "weekday": 5,
         "workingday": 1,
         "weathersit": 1, 
         "temp": 0.7, 
         "atemp": 0.65,
         "hum": 0.55,
         "windspeed": 0.25 
       }
     ]
  }
}

```
## Resultado.
```
[
  849.588704557757
]
```
6. Este JSON contém dados de entrada para o modelo de regressão. Agora, vamos enviar esses dados para o ponto de extremidade do modelo e ver qual é a previsão resultante.

Vamos analisar os dados de entrada que fornecemos ao modelo:

* "day": 10: Este valor representa o dia do mês.
* "mnth": 5: Refere-se ao mês (maio).
* "year": 2023: Indica o ano.
* "season": 1: Representa a estação do ano (no caso, primavera).
* "holiday": 0: Indica se é feriado ou não (0 para não feriado).
* "weekday": 5: Refere-se ao dia da semana (sexta-feira).
* "workingday": 1: Indica se é dia útil ou não (1 para dia útil).
* "weathersit": 1: Representa a condição climática (1 para clima limpo).
* "temp": 0.7: É a temperatura normalizada.
* "atemp": 0.65: É a temperatura aparente normalizada.
* "hum": 0.55: É a umidade normalizada.
* "windspeed": 0.25: É a velocidade do vento normalizada.

7. Conclusão:
Essa previsão indica que, com os dados de entrada fornecidos, o modelo estimou que haveria aproximadamente  849 aluguéis de bicicletas para o dia específico e as condições climáticas descritas. Essa previsão é útil para entender como o modelo responde a diferentes conjuntos de dados de entrada e pode ser usado para análises e tomada de decisões relacionadas ao aluguel de bicicletas.
