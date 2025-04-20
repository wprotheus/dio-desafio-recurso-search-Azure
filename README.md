# DIO - Trilha Java Básico

## Autor

🔸[wprotheus](https://github.com/wprotheus)

---

## Desafio - Azure Cognitive Search: Utilizando AI Search para indexação e consulta de Dados

Atividade executada conforme orientações abaixo, retiradas do [Descrição do Desafio](https://web.dio.me/lab/azure-cognitive-search-utilizando-ai-search-para-indexacao-e-consulta-de-dados/learning/719d6530-4d08-40c7-bb11-9524091868c0)  
<small><sup>Obs.: O link acima somente é acessado através de uma conta na plataforma DIO.</sup></small>

### Descrição do Desafio
#### Em -> CONTEÚDOS  
> Este laboratório tem como objetivo **aplicar técnicas de organização e pesquisa de documentos por meio da ingestão de dados e indexação utilizando ferramentas de inteligência artificial***. Durante as aulas, foram abordados três passos principais: ingestão de conteúdo para IA, criação de índices inteligentes e exploração prática dos dados organizados. O foco está em desenvolver uma compreensão sólida sobre como essas ferramentas podem ser utilizadas para minerar e extrair conhecimento de grandes volumes de informação. Como entregável, espera-se um **repositório estruturado contendo registros das etapas realizadas e insights obtidos ao longo da prática.**

#### Em -> INFORMAÇÕES  

> Neste LAB, aplicaremos técnicas de organização de documentos e conduziremos pesquisas eficientes através da ingestão de dados, seguindo três passos essenciais: ingestão de conhecimento de IA, criação do índice correspondente e exploração dessas funcionalidades. Ao final, ganharemos uma visão prática das potencialidades oferecidas por essas ferramentas na mineração de conhecimento.

### Objetivos de Aprendizagem  

> **Ao concluir este desafio, você será capaz de:**
> - Aplicar os conceitos aprendidos em um ambiente prático;
> - Documentar processos técnicos de forma clara e estruturada;
> - Utilizar o GitHub como ferramenta para compartilhamento de documentação técnica.
 
---  

# 🏗️ Criando uma Solução de Busca Inteligente com Azure AI Search

Este guia passo a passo mostra como configurar um ambiente básico no Microsoft Azure para utilizar o **Azure AI Search** com dados armazenados em um **Blob Storage**, ideal para testes e prototipação de soluções de IA aplicadas à análise de documentos.

---

## 🧱 Etapa 1: Criar o Recurso do Azure AI Search

1. Acesse o portal do Azure.
2. Clique em **+ Criar um recurso**.
3. Navegue até a categoria **AI + Machine Learning**.
4. Selecione **Azure AI Search**.
5. Clique em **Examinar + Criar**.
6. Configure os parâmetros obrigatórios:
    - Nome do recurso
    - Grupo de Recursos
    - Região
    - Plano de precificação (Free para testes)
7. Clique em **Criar**.

---

## 🤖 Etapa 2: Criar o Recurso Azure AI Services (para futuras análises cognitivas)

1. Clique em **+ Criar um recurso**.
2. Vá em **AI + Machine Learning**.
3. Selecione **Azure AI Services**.
4. Clique em **Examinar + Criar**.
5. Preencha as informações conforme necessário.
6. Finalize com **Criar**.

---

## 🗄️ Etapa 3: Criar uma Conta de Armazenamento

1. Clique em **+ Criar um recurso**.
2. Selecione a categoria **Armazenamento**.
3. Escolha **Conta de armazenamento**.
4. Clique em **Examinar + Criar**.
5. Configure:
    - Nome da conta
    - Região
    - Tipo de redundância
6. Clique em **Criar**.

---

## 📦 Etapa 4: Preparar o Armazenamento para os Dados

1. Após a conta ser criada, acesse o recurso.
2. Vá até **Contêineres**.
3. Clique em **+ Contêiner**.
4. Defina um nome (ex: `dados-analisados`).
5. No **Nível de acesso público**, selecione:
    - **Contêiner (acesso de leitura anônimo para contêineres e blobs)**.
6. Clique em **Criar**.
7. Acesse o contêiner recém-criado e faça o **upload dos dados** para análise (ex: arquivos PDF, imagens, documentos).

---

## 🔎 Etapa 5: Importar os Dados para o Azure AI Search

1. Vá até o recurso **Azure AI Search** criado anteriormente.
2. No menu lateral, clique em **Importar dados**.
3. Selecione como fonte de dados o **Azure Blob Storage**.
4. Configure a conexão com a conta de armazenamento:
    - Selecione a conta
    - Escolha o contêiner com os dados enviados
5. Prossiga com as configurações:
    - Nomeie o índice
    - Escolha o método de indexação (por exemplo, documentos)
6. Finalize com **Criar**.

---

## ✅ Pronto!

Você configurou com sucesso um pipeline básico para ingestão e análise de documentos usando **Azure AI Search** e **Azure Blob Storage**.

---

## 📷 Capturas de telas

### Tela #1:
<img src="./img_search/tela (1).png" alt="Tela criando recurso" width="350px"/>  

### Tela #2:
<img src="./img_search/tela (2).png" alt="Tela recurso criado" width="350px"/> 

### Tela #3:
<img src="./img_search/tela (3).png" alt="Tela criando recurso" width="350px"/>  

### Tela #4:
<img src="./img_search/tela (4).png" alt="Tela configurando recurso" width="350px"/>  

### Tela #5:
<img src="./img_search/tela (5).png" alt="Tela criando recurso" width="350px"/>  

### Tela #6:
<img src="./img_search/tela (6).png" alt="Tela adicionando contêiner" width="350px"/>  

### Tela #7:
<img src="./img_search/tela (7).png" alt="Tela visualização dados carregados" width="350px"/>  

### Tela #8:
<img src="./img_search/tela (8).png" alt="Tela configurando importação dados" width="350px"/>  
  
### Tela #9:  
<img src="./img_search/tela (9).png" alt="Tela resultado pesquisa" width="350px"/>  

---  

### 📘 **Documentações Recomendadas:**
- [Visão geral do Azure AI Search](https://learn.microsoft.com/pt-br/azure/search/search-what-is-azure-search) 
- [Criar um serviço do Azure AI Search](https://learn.microsoft.com/pt-br/azure/search/search-create-service-portal) 
- [O que são os Azure AI Services?](https://learn.microsoft.com/pt-br/azure/cognitive-services/cognitive-services-overview)  
- [Visão geral do Armazenamento do Azure](https://learn.microsoft.com/pt-br/azure/storage/common/storage-account-overview) 
- [Criar uma conta de armazenamento](https://learn.microsoft.com/pt-br/azure/storage/common/storage-account-create)   
- [Criar um contêiner no Azure Blob Storage](https://learn.microsoft.com/pt-br/azure/storage/blobs/storage-quickstart-blobs-portal) 
- [Upload de arquivos para Blob Storage](https://learn.microsoft.com/pt-br/azure/storage/blobs/storage-upload-process-images?tabs=azure-portal) 
- [Importar dados para Azure AI Search](https://learn.microsoft.com/pt-br/azure/search/search-howto-index-blob-storage)
- [Indexação de blobs com enriquecimento cognitivo (opcional)](https://learn.microsoft.com/pt-br/azure/search/cognitive-search-blob)
