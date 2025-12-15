# LSEG Solution Architect Interview Prep

## Skills Mapping: Your Experience → Job Requirements

| LSEG Requirement | Your Evidence |
|------------------|---------------|
| **Pre-sales & client engagement** | Bloomberg: MARS API demos for Japanese banks, APAC hedge funds; BQuant visualization presented at Tokyo seminar |
| **Build prototypes/POCs** | RFQ app (React/FastAPI) adopted by APAC Sales; This stock insights demo |
| **Generative AI/LLMs** | Georgia Tech Deep Learning + NLP courses; VLM fine-tuning research (51.5% ChartQA); Gemini integration |
| **Financial data** | 7+ years: Bloomberg MARS/DLIB, MSCI RiskMetrics, VaR, OTC derivatives |
| **Cloud platforms** | Azure (this project), AWS/GCP (academic DVA course), Databricks (Spark coursework) |
| **Microsoft Fabric** | Lakehouse pattern simulation - architecture ready for Fabric migration |
| **LangChain/RAG** | Implemented in this project with ChromaDB vector store |
| **Python** | Extensive: pandas, FastAPI, Streamlit, yfinance, plotly |
| **Japanese business level** | Native speaker - client engagement ready |
| **REST/GraphQL APIs** | Bloomberg MARS API, FastAPI backends |

## Key Talking Points

### Q: Walk us through this project
> "I built a stock insights dashboard demonstrating a Microsoft Fabric Lakehouse pattern using Azure Blob Storage. The app integrates yfinance for market data, Gemini for AI analysis, and implements RAG with LangChain for document-based Q&A. The architecture migrates directly to Fabric."

### Q: Why simulate Fabric instead of using it?
> "Fabric requires enterprise licensing. By using Azure Blob with Parquet files, I demonstrate the same patterns - data lake storage, columnar format, separation of compute and storage. The code abstractions make migration straightforward: swap BlobServiceClient for FabricClient, Parquet for Delta."

### Q: How would you use this for LSEG clients?
> "This demonstrates rapid prototyping value. For client workshops, I'd adapt this to integrate LSEG data - Refinitiv market data, World-Check for KYC, or Workspace APIs. The RAG component could surface LSEG research during analysis."

### Q: Tell us about your pre-sales experience
> "At Bloomberg, I collaborated with Sales to scope MARS API solutions for Japanese banks and APAC hedge funds. I built and presented a BQuant risk dashboard at a Tokyo industry seminar. My RFQ prototype using React/FastAPI was adopted by APAC Sales for client demos. I authored Python integrations that accelerated client adoption 2x."

### Q: Experience with AI-assisted development?
> "I'm a power user of Claude Code and GitHub Copilot for rapid prototyping. I focus on business logic while AI handles boilerplate. This methodology accelerates POC delivery significantly."

### Q: How do you handle client workshops?
> "At Bloomberg and MSCI, I led technical discovery sessions to understand client challenges. I translate requirements into solution architectures, build working prototypes, and present technical feasibility to stakeholders. I've done this for 30+ clients in the APAC region."

## Demo Script (5 minutes)

**[0:00-0:30] INTRO**
"This is a stock insights POC demonstrating Fabric Lakehouse patterns with GenAI."

**[0:30-1:30] DATA LAYER**
- Show sidebar: Azure Blob connection status
- Explain: "Container = Lakehouse, Parquet = Delta tables"
- Show code: DataLakeStorage class abstraction

**[1:30-2:30] AI ANALYSIS**
- Enter ticker, click "Generate AI Insights"
- While loading: "Using Gemini with structured prompts"
- Show analysis output

**[2:30-3:30] RAG DEMONSTRATION**
- Switch to RAG tab
- Ask: "What are the key risks for AAPL?"
- Explain: "LangChain retrieves relevant analyst reports, Gemini synthesizes"

**[3:30-4:30] FABRIC MIGRATION PATH**
- Open ARCHITECTURE.md
- Walk through migration table
- "Production: OneLake, Delta, Eventstream"

**[4:30-5:00] CLOSING**
"This demonstrates rapid prototyping of AI-enabled financial applications - exactly what I'd do for LSEG client POCs."

## Questions to Ask Them

1. "What's the typical client engagement cycle - from discovery to production deployment?"
2. "Which LSEG data products are most commonly integrated into AI solutions?"
3. "How does the team balance pre-sales work with delivery responsibilities?"
4. "What's the current adoption of Microsoft Fabric among LSEG clients?"
