![github-repository-share_shadow-monster](https://github.com/user-attachments/assets/fc0d4703-c9b5-4320-969f-c234c9d4b979)

## 👻 Caça aos Bugs 2025 - Desafio 08 - Shadow Monster

Oi, eu sou o Edilson Ribeiro e este é o espaço onde compartilho minha jornada de aprendizado durante o desafio **Caça aos Bugs 2025**, realizado pelo [balta.io](https://balta.io). 👻

Aqui você vai encontrar projetos, exercícios e códigos que estou desenvolvendo durante o desafio. O objetivo é colocar a mão na massa, testar ideias e registrar minha evolução no mundo da tecnologia.

### Sobre este desafio
No desafio **Shadow Monster** eu tive que fazer a publicação da aplicação utilizando o processo de CI/CD com GitHub Actions.
Neste processo eu aprendi:
* ✅ Git e GitHub
* ✅ CI/CD
* ✅ Build e Test
* ✅ GitHub Actions
* ✅ Microsoft Azure

## REGRAS DO DESAFIO
- [x] Realizar um fork do repositório do desafio
- [x] Criar um Workflow para branch main
- [x] Executar o build do projeto no Workflow
- [x] Executar o teste (Unit Test) do projeto no Workflow
- [x] Realizar o deployment automatizado da aplicação via CI/CD

### Deploy automatizado no Azure App Service
O Workflow `CI` compila, testa, publica e faz o deploy da API automaticamente na branch `main`. Para habilitar o deploy, siga estes passos:

1. Crie um Azure App Service (Plano F1 gratuito é suficiente) e baixe o *Publish Profile* da aplicação.
2. No GitHub, acesse `Settings > Secrets and variables > Actions` e cadastre:
   * Secret `AZURE_WEBAPP_PUBLISH_PROFILE` com o conteúdo completo do publish profile.
   * Variable `AZURE_WEBAPP_NAME` com o nome exato da sua App Service.
3. Faça um push na branch `main`. O workflow `CI` vai:
   * restaurar dependências, compilar e testar a solução,
   * executar `dotnet publish` gerando os artefatos em `published-app`,
   * enviar os artefatos para o Azure usando `azure/webapps-deploy`.
4. Acompanhe a execução em `Actions`. Ao finalizar sem erros, a aplicação estará disponível no Azure App Service recém configurado.

## Sobre o Caça aos Bugs
O desafio **Caça aos Bugs 2025** consiste em encontrar bugs e sugerir melhorias para aplicações em cenários reais. Durante os 9 desafios desta jornada, os participantes são submetidos ao aprendizado e prática de Depuração de Aplicações, Testes de Unidade, Testes E2E, Melhorias de UI, Melhorias de Performance, Deployment e Infraestrutura,
Banco de Dados.

### Veja meu progresso no desafio
[Incluir link para o repositório central]
