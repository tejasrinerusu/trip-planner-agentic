# ✈️ AI Travel Planner – Agentic AI Application

An AI-powered travel planning application that generates personalized trip itineraries using an agentic AI workflow.

## 🌐 Live Demo

🚀 **Try the application:**  
https://trip-planner-agentic-n2cexl4az9gsw5jytck9gu.streamlit.app/

## 📌 Overview

The AI Travel Planner helps users plan trips by generating detailed travel itineraries based on their requirements.

The application uses an agentic workflow where an AI agent can use different tools to:

- Plan day-by-day travel itineraries
- Search for attractions
- Estimate hotel expenses
- Calculate total expenses
- Calculate daily travel budgets
- Provide travel recommendations
- Generate personalized trip plans

## 🛠️ Tech Stack

- **Python**
- **Streamlit** – Frontend
- **FastAPI** – Backend API
- **LangChain** – Agentic AI framework
- **LangGraph** – Agent workflow orchestration
- **Groq** – LLM inference
- **Google APIs** – Travel and location-related tools
- **Uvicorn** – ASGI server
- **Git & GitHub** – Version control
- **Render** – Backend deployment
- **Streamlit Community Cloud** – Frontend deployment

## 🏗️ Architecture

```text
                    User
                      │
                      ▼
          ┌─────────────────────┐
          │   Streamlit Cloud   │
          │      Frontend       │
          └──────────┬──────────┘
                     │
                     │ POST /query
                     ▼
          ┌─────────────────────┐
          │   FastAPI Backend   │
          │       Render        │
          └──────────┬──────────┘
                     │
                     ▼
          ┌─────────────────────┐
          │   Agentic Workflow  │
          │ LangChain/LangGraph │
          └──────────┬──────────┘
                     │
              ┌──────┴──────┐
              ▼             ▼
            Groq       External APIs
