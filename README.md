# Azure Cognitive Search — Visão Geral

O **Azure Cognitive Search** é um serviço da Microsoft Azure que permite **criar experiências de busca personalizadas** para aplicativos, sites ou sistemas internos. Ele funciona como um **"motor de busca como serviço"** (Search-as-a-Service), oferecendo uma infraestrutura pronta para indexar, buscar e analisar dados de forma inteligente.

---

## 🔧 Como Funciona (Passo a Passo)

### 1. Fonte de dados (Data Source)
Você conecta o Azure Cognitive Search a uma fonte de dados, como:
- Azure SQL Database
- Azure Blob Storage
- Cosmos DB
- SharePoint
- Documentos (PDF, DOCX etc.)

### 2. Indexador (Indexer)
O indexador coleta os dados da fonte e os transforma em um **índice de busca** pesquisável.

### 3. Habilidades cognitivas (Cognitive Skills) — opcional
Durante a indexação, você pode aplicar IA para enriquecer os dados com:
- OCR (extração de texto de imagens)
- Detecção de linguagem
- Extração de entidades (pessoas, lugares, datas)
- Tradução automática
- Análise de sentimentos

Essas habilidades compõem o chamado **pipeline de enriquecimento cognitivo**.

### 4. Índice de busca (Search Index)
O índice é onde os dados ficam armazenados de forma otimizada para buscas rápidas. Nele você define:
- Campos pesquisáveis
- Campos filtráveis
- Campos ordenáveis

### 5. API de busca
Você consulta os dados via API REST ou SDKs (C#, Python, etc), usando:
- Pesquisa textual (full-text search)
- Filtros (por categorias, faixas de preço, etc)
- Ordenações
- Sugestões automáticas (autocomplete)

---

## 📊 Diagrama Simplificado

```text
[Fonte de Dados] 
      ↓
[Indexador] 
      ↓
[Habilidades Cognitivas (opcional)]
      ↓
[Índice de Busca]
      ↓
[API de Busca]
