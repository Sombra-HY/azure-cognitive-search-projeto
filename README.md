# Azure Cognitive Search: Utilizando AI Search para Indexação e Consulta de Dados

## Objetivo

Este projeto tem como foco a configuração e uso do Azure AI Search (Cognitive Search) para indexar e consultar dados de maneira inteligente, aproveitando os recursos de Inteligência Artificial da plataforma Azure.

---

## Passo a Passo da Configuração

### 1. Criar um Serviço de Azure Cognitive Search

- Acesse o [Portal Azure](https://portal.azure.com)
- Vá em **Criar recurso** > **Web** > **Azure Cognitive Search**
- Escolha:
  - Nome do serviço
  - Região
  - Camada de precificação (Free F1 para testes)
- Clique em **Criar**

### 2. Subir um Dataset

- Utilize Azure Blob Storage ou envie arquivos JSON/CSV manualmente
- Pode incluir documentos como: PDF, DOCX, CSV ou JSON

### 3. Criar um Indexador e um Index

- No serviço criado, vá em **Importar dados**
- Selecione a origem dos dados
- Configure o **Indexador** (responsável por puxar os dados)
- Configure o **Index** (estrutura que define os campos a serem pesquisados)
- Ative o recurso de **AI Enrichment** para aplicar:
  - Leitura de imagens e PDFs (OCR)
  - Análise de sentimentos
  - Extração de entidades nomeadas

### 4. Criar um Search Client (Consulta)

- Utilize Postman, cURL ou SDKs (.NET, Python, JavaScript)
- Endpoint base:## Aplicações, Benefícios e Aprendizados

O uso do **Azure Cognitive Search** pode ser aplicado a diversas situações que exigem busca inteligente em grandes volumes de dados. Algumas aplicações práticas incluem:

- **Chatbots com base em conhecimento**: fornecem respostas precisas indexando conteúdos de ajuda.
- **Sistemas de FAQ automatizados**: buscam respostas em bases de dados dinâmicas.
- **Plataformas de busca interna corporativa**: ajudam equipes a encontrar documentos com agilidade.
- **Sistemas jurídicos para consulta de jurisprudência**: realizam buscas semânticas em textos legais.
- **Suporte técnico ao cliente**: facilitam o acesso rápido a manuais, tutoriais e bases de conhecimento.

Essas soluções se beneficiam dos recursos oferecidos pelo Cognitive Search, como:

- **Busca textual inteligente (full-text search)** com filtros, ordenações e fuzzy search.
- **Integração com serviços como** Power BI, Logic Apps, Power Automate, Web Apps e aplicações móveis.
- **Enriquecimento com IA (AI Enrichment)**: OCR, extração de entidades, análise de sentimentos e tradução.

### Aprendizados

Durante a construção deste projeto, foram adquiridos os seguintes aprendizados:

- Estruturar e indexar dados não estruturados (como PDF, DOCX e JSON).
- Usar enriquecimento de IA para extrair valor dos dados.
- Criar APIs de busca seguras com autenticação por `api-key`.
- Compreender a arquitetura e os componentes do Azure Cognitive Search.
- Aplicar boas práticas de segurança, escalabilidade e integração em soluções de busca.
