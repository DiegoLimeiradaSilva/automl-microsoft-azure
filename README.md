
**Trabalhando com Machine Learning na Prática no Azure ML**

# automl-microsoft-azure

- Passo a passo de experimento de Aprendizagem Automatizada, de Regressão, utilizando A **Azure Machine Learning**, realizado como desafio de projeto no Bootcamp **Microsoft Azure AI Fundamentals** da [Dio.me](https://dio.me)

<br/>

## Passo 1

- Criar uma conta no [https://azure.microsoft.com/pt-br/free](https://azure.microsoft.com/pt-br/free)
- O cadastro é inicializado ao clicar no botão "Experimentar gratuitamente" É necessário informar um número de cartão de crédito para validacao da conta com valor [***irrisório***](https://www.google.com/search?sca_esv=529a5e0a05223c39&rlz=1C5CHFA_enBR1091BR1091&sxsrf=ACQVn0-tQrWQ9cVQlNvbdRlqbAXl5G_EEQ:1708232569331&q=irris%C3%B3rio&spell=1&sa=X&ved=2ahUKEwiigPSbjrSEAxU7q5UCHdh-CeEQkeECKAB6BAgHEAI), que será extornado/
- ![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/01.png?raw=true)

## Passo 2

- Acessar a plataforma do Azure em [portal.azure.com](portal.azure.com)
- Buscar por "Azure Machine Learning" no campo de busca e selecionar o card referido.

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/2.png?raw=true)

## Passo 3

- Clicar em "Criar", para criar um novo workspace

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/3.png?raw=true)

## Passo 4

- Criar um novo "resource group", criar um "nome", a "região", e clicar em "Examinar e criar"

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/4.png?raw=true)

- Aguardar até que a validação seja aprovada, e então clicar em "criar"

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/5.png?raw=true)

## Passo 5

- A implantação fica em andamento e pode ser acompanhada na tela que é aberta automaticamente

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/6.png?raw=true)

- Esta é a tela de finalização do deploy. Agora podemos clicar em "ir para o recurso".

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/7.png?raw=true)

- Na tela do recurso, clicar em "Iniciar estúdio"

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/8.png?raw=true)

## Passo 6

- O diretório do workspace é então aberto.
- Posso visualizar todos os workspaces existentes, clicando em "all workspaces"

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/9.png?raw=true)

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/10.png?raw=true)

## Passo 7

- O workspace escolhido é aberto. Preciso agora entrar no ambiente "Automated ML" e clicar em criar um "new ML automated job"

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/11.png?raw=true)

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/12.png?raw=true)

## Passo 7

- Preencher os dados do job com as informações (fornecidas pela documentação da Microsoft)
- 7.1 -> Preenchimento das informações básicas

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/13.png?raw=true)

- 7.2 -> Escolha do tipo de tarefa (Regressão) e criação do dataset

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/14.png?raw=true)

- 7.3 -> Preenchimento das informações do dataset

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/15.png?raw=true)

- 7.4 -> Escolha da fonte dos dados

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/16.png?raw=true)

- 7.5 -> Inclusão da url do dataset. A url passa por uma verificação e validação.

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/17.png?raw=true)

- 7.6 -> Os dados devem estar com as seguintes configurações

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/18.png?raw=true)

- 7.7 -> Ele traz uma visualização do schema. Não é necessário alterar nenhuma informação.

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/19.png?raw=true)

- 7.8 -> Por fim, ele traz todas informações para review, e clicamos em "criar", para criar o dataset.

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/20.png?raw=true)

- 7.9 -> Para avançar, selecionamos o dataset, e clicamos em "next"

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/21.png?raw=true)

- 7.10 -> Configurações da tarefa

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/22.png?raw=true)

- 7.11 -> Não é necessário setar nenhuma informação diferença da parte de Computação

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/23.png?raw=true)

- 7.12 -> As informações são trazidas e podemos enviar o trabalho de treinamento

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/24.png?raw=true)

## Passo 8

- O modelo inicia o treinamento até a finalização

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/25.png?raw=true)

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/26.png?raw=true)

## Passo 9

- Validar métricas
- 9.1 -> Acessar as informações do modelo conforme imagem abaixo
  ![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/27.png?raw=true)
- 9.2 -> Acessar o job

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/28.png?raw=true)

- 9.3 -> Acessar as métricas

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/29.png?raw=true)

- As métricas trazem dois gráficos, o predicted_true e o residuals, que trazem informações de valores previstos comparados com os reais

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/30.png?raw=true)

## Passo 10

- Deploy e Teste do Modelo
- 10.1 -> De volta à página do modelo, escolhemos a opção de Deploy Web Service.

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/31.png?raw=true)

- 10.2 -> Preencher com as informações fornecidas na documentação e clicar em "Deploy"

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/32.png?raw=true)

- 10.3 -> Receberemos a notificação de que o deploy está completo e, no menu esquerdo, vamos clicar na aba Endpoints.

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/33.png?raw=true)

- 10.4 -> Na tela de Endpoint, confirmamos o status "Succeed" do deploy, e clicamos na aba "Test"

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/34.png?raw=true)

- 10.4 -> Substituímos o json existente, pelo código fornecido pela documentação, e depois clicamos em "Test".

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/35.png?raw=true)

- 10.5 -> Resultado do Teste

![image](https://github.com/DiegoLimeiradaSilva/automl-microsoft-azure/blob/main/imagens/36.png?raw=true)

## Códigos

<details>
<summary>Input (Clique para abrir)</summary>

```
 {
   "Inputs": { 
     "data": [
       {
         "day": 1,
         "mnth": 1,   
         "year": 2022,
         "season": 2,
         "holiday": 0,
         "weekday": 1,
         "workingday": 1,
         "weathersit": 2, 
         "temp": 0.3, 
         "atemp": 0.3,
         "hum": 0.3,
         "windspeed": 0.3 
       }
     ]  
   },   
   "GlobalParameters": 1.0
 }
```

</details>

<details>
<summary>Resultado (Clique para abrir)</summary>

```
{
  "Results": [
    331.839379193704
  ]
}
```

</details>

<details>
<summary>Swagger URI (Clique para abrir)</summary>

```
// 20240206030758
// http://ca6e07b7-d4a1-4ad1-8c57-489dfd4c6228.eastus.azurecontainer.io/swagger.json

{
  "swagger": "2.0",
  "info": {
    "title": "predict-rentals",
    "description": "API specification for the Azure Machine Learning service predict-rentals",
    "version": "1.0"
  },
  "schemes": [
    "https"
  ],
  "consumes": [
    "application/json"
  ],
  "produces": [
    "application/json"
  ],
  "securityDefinitions": {
    "Bearer": {
      "type": "apiKey",
      "name": "Authorization",
      "in": "header",
      "description": "For example: Bearer abc123"
    }
  },
  "paths": {
    "/": {
      "get": {
        "operationId": "ServiceHealthCheck",
        "description": "Simple health check endpoint to ensure the service is up at any given point.",
        "responses": {
          "200": {
            "description": "If service is up and running, this response will be returned with the content 'Healthy'",
            "schema": {
              "type": "string"
            },
            "examples": {
              "application/json": "Healthy"
            }
          },
          "default": {
            "description": "The service failed to execute due to an error.",
            "schema": {
              "$ref": "#/definitions/ErrorResponse"
            }
          }
        }
      }
    },
    "/score": {
      "post": {
        "operationId": "RunMLService",
        "description": "Run web service's model and get the prediction output",
        "security": [
          {
            "Bearer": [
        
            ]
          }
        ],
        "parameters": [
          {
            "name": "serviceInputPayload",
            "in": "body",
            "description": "The input payload for executing the real-time machine learning service.",
            "schema": {
              "$ref": "#/definitions/ServiceInput"
            }
          }
        ],
        "responses": {
          "200": {
            "description": "The service processed the input correctly and provided a result prediction, if applicable.",
            "schema": {
              "$ref": "#/definitions/ServiceOutput"
            }
          },
          "default": {
            "description": "The service failed to execute due to an error.",
            "schema": {
              "$ref": "#/definitions/ErrorResponse"
            }
          }
        }
      }
    },
    "/swagger.json": {
      "get": {
        "operationId": "GetSwaggerSpec",
        "description": "Get the Swagger specification.",
        "parameters": [
          {
            "name": "version",
            "in": "query",
            "required": false,
            "type": "integer",
            "enum": [
              2,
              3
            ]
          }
        ],
        "responses": {
          "200": {
            "description": "The Swagger specification.",
            "schema": {
              "type": "string"
            }
          },
          "default": {
            "description": "The service failed to execute due to an error.",
            "schema": {
              "$ref": "#/definitions/ErrorResponse"
            }
          }
        }
      }
    }
  },
  "definitions": {
    "ServiceInput": {
      "type": "object",
      "properties": {
        "Inputs": {
          "type": "object",
          "required": [
            "data"
          ],
          "properties": {
            "data": {
              "type": "array",
              "items": {
                "type": "object",
                "required": [
                  "day",
                  "mnth",
                  "year",
                  "season",
                  "holiday",
                  "weekday",
                  "workingday",
                  "weathersit",
                  "temp",
                  "atemp",
                  "hum",
                  "windspeed"
                ],
                "properties": {
                  "day": {
                    "type": "integer",
                    "format": "int64"
                  },
                  "mnth": {
                    "type": "integer",
                    "format": "int64"
                  },
                  "year": {
                    "type": "integer",
                    "format": "int64"
                  },
                  "season": {
                    "type": "integer",
                    "format": "int64"
                  },
                  "holiday": {
                    "type": "integer",
                    "format": "int64"
                  },
                  "weekday": {
                    "type": "integer",
                    "format": "int64"
                  },
                  "workingday": {
                    "type": "integer",
                    "format": "int64"
                  },
                  "weathersit": {
                    "type": "integer",
                    "format": "int64"
                  },
                  "temp": {
                    "type": "number",
                    "format": "double"
                  },
                  "atemp": {
                    "type": "number",
                    "format": "double"
                  },
                  "hum": {
                    "type": "number",
                    "format": "double"
                  },
                  "windspeed": {
                    "type": "number",
                    "format": "double"
                  }
                }
              },
              "format": "pandas.DataFrame:records"
            }
          }
        },
        "GlobalParameters": {
          "type": "number",
          "format": "double"
        }
      },
      "example": {
        "Inputs": {
          "data": [
            {
              "day": 0,
              "mnth": 0,
              "year": 0,
              "season": 0,
              "holiday": 0,
              "weekday": 0,
              "workingday": 0,
              "weathersit": 0,
              "temp": 0.0,
              "atemp": 0.0,
              "hum": 0.0,
              "windspeed": 0.0
            }
          ]
        },
        "GlobalParameters": 1.0
      }
    },
    "ServiceOutput": {
      "type": "object",
      "required": [
        "Results"
      ],
      "properties": {
        "Results": {
          "type": "array",
          "items": {
            "type": "integer",
            "format": "int64"
          },
          "format": "numpy.ndarray"
        }
      },
      "example": {
        "Results": [
          0
        ]
      }
    },
    "ErrorResponse": {
      "type": "object",
      "properties": {
        "message": {
          "type": "string"
        }
      }
    }
  }
}
```

</details>
