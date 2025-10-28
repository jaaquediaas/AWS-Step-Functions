# AWS-Step-Functions
Projeto Base: Explorando Workflows Automatizados com AWS Step Functions

# Automação de Workflows com AWS Step Functions

---

**📘 Sobre o Projeto**
---
Este laboratório teve como objetivo automatizar processos serverless utilizando o **AWS Step Functions**, orquestrando diferentes serviços da AWS como **Lambda**, **S3** e **DynamoDB**.

O foco foi compreender como modelar fluxos inteligentes e monitoráveis, reduzindo a complexidade operacional e aumentando a eficiência das execuções automatizadas.

---

**Metas de Aprendizagem**

* Entender o papel do AWS Step Functions dentro do ecossistema serverless.
* Criar e gerenciar máquinas de estados (*state machines*) com tarefas e decisões.
* Integrar funções Lambda e outros serviços AWS em fluxos automatizados.
* Adotar boas práticas de documentação e versionamento usando GitHub.

---

**🧠 Conceitos Fundamentais**
O AWS Step Functions é um serviço de orquestração baseada em estados, onde cada etapa representa uma ação específica dentro de um fluxo.
Ele permite modelar processos complexos como fluxos visuais, sem precisar escrever código de controle ou gerenciar infraestrutura manualmente.

---
**🧱 Arquitetura do Laboratório**

Durante o laboratório, foi desenvolvido um fluxo de automação no AWS Step Functions responsável por processar atualizações de produtos a partir de arquivos JSON armazenados no S3.

O fluxo segue as seguintes etapas:

-ProcessProductUpdates (Map State) — Lê e percorre o arquivo updates/product-updates.json, processando cada item individualmente.

-ValidateAndUpdateProduct (Lambda) — Executa uma função Lambda que valida os dados e aplica as regras de atualização dos produtos.

-UpdateDynamoDB (DynamoDB UpdateItem) — Atualiza os registros validados diretamente em uma tabela do Amazon DynamoDB.

Exportação de Resultados — Os resultados são armazenados no bucket configurado em <S3_RESULT_BUCKET>.

---

**💡 Insights**
---
Durante o laboratório, foi possível perceber como o Step Functions simplifica a orquestração de processos serverless, garantindo fluxos consistentes, visíveis e de fácil manutenção.
A automação reduz erros, melhora o controle e libera tempo para o foco no desenvolvimento da lógica de negócio.

---



---

Pronto para postar! Quer que eu te adicione uma **linha de descrição curta** (para colocar na parte “About” do repositório no GitHub)?
