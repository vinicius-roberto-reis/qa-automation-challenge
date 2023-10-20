# 🚀 Projeto de Teste com Newman

Este é um projeto de teste automatizado usando a ferramenta Newman para testar uma API. O projeto demonstra como configurar, executar e gerar relatórios para testes de API.

## 🛠️ Ferramentas Utilizadas

- [Node.js](https://nodejs.org/): Plataforma para executar JavaScript.
- [Postman](https://www.postman.com/): Ferramenta para criar, testar e documentar APIs.
- [Newman](https://learning.postman.com/docs/running-collections/using-newman-cli/integration-with-jenkins/): CLI para Postman, usado para executar coleções de testes e gerar relatórios.

## 📦 Instalação

Certifique-se de ter Node.js instalado antes de começar.

1. Clone este repositório:

   ```bash
   git clone https://github.com/vinicius-roberto-reis/qa-automation-challenge.git
   ```

2. Acesse a pasta do projeto:
   ```bash
   cd qa-automation-challenge
   ```

3. Instale o Newman globalmente (caso ainda não tenha instalado):
   ```bash
   npm install -g newman
   ```

## 🚀 Executando Testes Localmente
Para executar os testes localmente, siga as etapas abaixo:

Abra um terminal na pasta do projeto.

Execute o seguinte comando para executar os testes:

 ```bash
newman run JsonPlaceholderTests.postman_collection.json -r html --reporter-html-export report.html```

Após a execução, o relatório será gerado e disponível para revisão.

## 🚀 Executando Testes com o GitHub Actions (Manual)
Este projeto também inclui um fluxo de trabalho de integração contínua (CI) usando GitHub Actions. No entanto, este fluxo de trabalho é manual, o que significa que você deve acioná-lo explicitamente quando desejar executar os testes. Siga os passos abaixo:

Abra o GitHub e acesse o seu repositório.

No repositório, clique na guia "Actions" na parte superior.

No lado esquerdo, você verá "Workflows" disponíveis. Clique em "Execution Automation Workflow" para abrir o fluxo de trabalho.

Clique no botão "Run workflow" para iniciar a execução dos testes.

Aguarde até que o GitHub Actions execute os testes. Os resultados serão disponibilizados no final da execução.

## 📊 Gerando Relatórios
Os relatórios dos testes serão gerados em formato HTML no proprio job que foi executado. Você pode abrir o arquivo HTML em qualquer navegador para visualizar os resultados dos testes.
   
