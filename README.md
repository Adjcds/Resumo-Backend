# Estudos de Back End com Ênfase em APIs

## Introdução

Este repositório é dedicado aos meus estudos voltados para o desenvolvimento de aplicações back end, com foco especial em APIs (Interfaces de Programação de Aplicações). Aqui, compartilho conceitos, exemplos práticos e aprendizados relacionados à construção e consumo de APIs, assim como a implementação de APIs RESTful.

## API: Conceitos Fundamentais

Uma API (Interface de Programação de Aplicações) é um conjunto de regras e definições que permite a comunicação entre diferentes softwares. Ela desempenha um papel crucial no desenvolvimento de sistemas distribuídos, facilitando a integração e o intercâmbio de dados entre aplicações.

### Exemplo de Utilização de API

Para ilustrar o conceito, considere uma API de previsão do tempo, onde um aplicativo pode requisitar informações sobre as condições climáticas atuais e previsões futuras.

```python
# Exemplo de requisição usando Python
import requests

url = "https://api.weather.com/forecast"
params = {
    "city": "example_city",
    "api_key": "your_api_key"
}

response = requests.get(url, params=params)
weather_data = response.json()

print(weather_data)

## APIs RESTful: Estrutura e Convenções

As APIs RESTful seguem princípios arquiteturais que favorecem a simplicidade, escalabilidade e a padronização. Aqui estão as regras fundamentais divididas em quatro categorias:

### 1. Endpoints

Os endpoints são URLs que representam recursos ou objetos no sistema. Eles definem onde as solicitações podem ser feitas.

### 2. Verbos HTTP

Os verbos HTTP (GET, POST, PUT, PATCH, DELETE) indicam a operação que deve ser realizada no recurso. Aqui está uma tabela exemplificando o uso desses verbos:

| Verbo  | URL                                 | Finalidade                      |
|--------|-------------------------------------|---------------------------------|
| GET    | https://api.com.br/produtos/2       | Obter um produto                |
| GET    | https://api.com.br/produtos/         | Obter todos os produtos         |
| POST   | https://api.com.br/produtos/         | Cadastrar um produto            |
| PUT    | https://api.com.br/produtos/2       | Atualizar todos os dados        |
| PATCH  | https://api.com.br/produtos/2       | Atualizar alguns dados          |
| DELETE | https://api.com.br/produtos/2       | Excluir um produto              |

### 3. JSON

O formato de dados comum em APIs RESTful é o JSON (JavaScript Object Notation). Ele é utilizado para representar e transmitir dados entre cliente e servidor de maneira leve e eficiente.

### 4. Códigos de Status

Os códigos de status HTTP indicam o resultado de uma operação. Exemplos incluem 200 (OK), 201 (Created), 204 (No Content), 400 (Bad Request), 404 (Not Found), entre outros.

## Postman: Testando e Documentando APIs

O Postman é uma ferramenta poderosa para testar e documentar APIs. Ele simplifica a execução de requisições HTTP, permitindo explorar e entender o comportamento de uma API.

### Exemplo de Utilização do Postman

1. Importe a coleção do Postman disponível neste repositório.
2. Explore os diferentes endpoints e verbos HTTP.
3. Observe os dados de requisição e resposta, incluindo códigos de status.

