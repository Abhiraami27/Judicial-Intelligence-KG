# ⚖️ Judicial Intelligence Knowledge Graph

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python" />
  <img src="https://img.shields.io/badge/FastAPI-Backend-009688?style=for-the-badge&logo=fastapi" />
  <img src="https://img.shields.io/badge/React-Frontend-61DAFB?style=for-the-badge&logo=react" />
  <img src="https://img.shields.io/badge/Neo4j-Knowledge%20Graph-4581C3?style=for-the-badge&logo=neo4j" />
  <img src="https://img.shields.io/badge/Groq-AI-orange?style=for-the-badge" />
</p>

<p align="center">
  <b>AI-powered legal case exploration and judicial knowledge graph platform</b>
</p>

---

## 📌 Overview

**Judicial Intelligence Knowledge Graph** is a full-stack legal intelligence platform designed to transform judicial case information into an interactive, searchable knowledge graph.

The system combines:

- 🧠 AI-assisted legal keyword extraction
- 🔎 IndianKanoon case search
- 🕸️ Neo4j knowledge graph visualization
- 📄 PDF/TXT judicial document ingestion
- ⚖️ Case, court, party and order relationships
- 📊 Judicial analytics and dashboard metrics
- 🔗 Related-case discovery
- 📚 Graph history and case exploration
- 🌐 React-based interactive frontend
- ⚡ FastAPI backend services

The platform allows users to upload a judicial document, extract relevant legal concepts, search for related cases, and visualize relationships between cases, courts, parties and orders.

---

# 🚀 Key Features

## 🧠 AI-Assisted Legal Analysis

Uploaded judicial documents are processed to identify meaningful legal keywords.

The system can:

- Extract text from uploaded documents
- Generate legal keyword candidates
- Finalize a set of legal search keywords
- Match keywords against candidate cases
- Rank relevant case results
- Fall back to heuristic keyword processing when AI services are unavailable

The Groq integration is configurable through environment variables and is designed to generate a fixed set of legal search keywords and evaluate case relevance. 

---

## 📄 Judicial Document Upload

Users can upload:

- PDF files
- TXT files

The upload pipeline performs:

```text
Document Upload
      ↓
File Validation
      ↓
Text Extraction
      ↓
Legal Keyword Extraction
      ↓
AI Keyword Finalization
      ↓
IndianKanoon Search
      ↓
Case Matching
      ↓
Neo4j Graph Creation
      ↓
Interactive Graph Visualization
