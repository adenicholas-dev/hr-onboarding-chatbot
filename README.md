# HR Onboarding Chatbot — AI-Powered RAG Pipeline

An intelligent HR assistant built with n8n, Pinecone, and Google Gemini.

## What It Does
- Automatically ingests HR policy documents from Google Drive
- Stores them as vectors in Pinecone Vector Database
- Answers employee HR questions via an AI chat interface

## Tech Stack
- n8n (workflow automation)
- Pinecone (vector database)
- Google Gemini (AI model + embeddings)
- Google Drive (document storage)

## Architecture
Pipeline 1 — Document Ingestion:
Google Drive Trigger → Download File → Default Data Loader → Embeddings → Pinecone

Pipeline 2 — Chatbot:
Chat Trigger → AI Agent → Pinecone (retrieval) + Gemini (response generation)

## Use Case
Companies can upload HR documents to Google Drive and employees 
can instantly ask questions about leave policy, benefits, 
code of conduct and get accurate AI-powered answers.
