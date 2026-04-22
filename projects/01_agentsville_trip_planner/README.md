# 🧠 AgentsVille Trip Planner

An AI-powered travel planning assistant that generates, evaluates, and refines personalized itineraries using Large Language Models (LLMs) and agent-based reasoning.

---

## 📌 Overview

Welcome to the **AgentsVille Trip Planner** — a multi-stage AI system where you take on the role of an AI Engineer to design a smart travel assistant.

This project simulates a traveler planning a trip to the fictional city of **AgentsVille**, with specific preferences such as:

- Duration (weekend / full week)
- Interests (art, tech, culture, food, etc.)
- Budget constraints

The system goes beyond simple text generation. It **understands**, **plans**, and **iteratively improves** travel itineraries using reasoning and tool interaction.

---

## 🎯 Objectives

The system is designed to:

### 1. Understand & Interpret
- Parse user preferences and constraints
- Extract meaningful travel requirements

### 2. Plan Comprehensively
- Generate a structured, day-by-day itinerary
- Ensure coherence and personalization

### 3. Evaluate & Enhance
- Improve the itinerary using tools and reasoning
- Adapt to follow-up queries and changes

---

## 🏗️ Project Architecture

The project consists of two major components:

---

### 🧭 1. Expert Planner (Initial Itinerary Generator)

**Goal:** Create a complete travel plan based on user input.

#### Responsibilities:
- Accept user inputs:
  - Destination (AgentsVille)
  - Duration
  - Interests
  - Budget
- Prompt the LLM to act as a travel expert
- Generate a **structured itinerary**

#### Output:
- A **JSON itinerary**
- Must conform to a predefined **Pydantic model**

#### Key Focus:
- Prompt engineering
- Structured output generation
- Planning logic

---

### 🤖 2. Resourceful Assistant (ReAct Agent for Enhancement)

**Goal:** Improve and adapt the itinerary dynamically.

#### Responsibilities:
- Handle follow-up user requests
- Analyze current itinerary context
- Decide whether external tools are needed

#### Agent Workflow (ReAct Pattern):

1. **THINK**
   - Analyze the request
   - Plan next steps

2. **ACT**
   - Call a tool (e.g., simulated activities API)

3. **OBSERVE**
   - Receive tool output

4. **RESPOND**
   - Update itinerary or answer user

#### Capabilities:
- Modify plans
- Add/remove activities
- Optimize schedule
- Incorporate external data

---

## 🛠️ Tech Stack

- **Python**
- **Jupyter Notebook**
- **LLM (e.g., OpenAI / compatible models)**
- **Pydantic** (for schema validation)
- **ReAct Agent Pattern**

---

## 🔑 Key Learning Outcomes

- Prompt engineering for structured outputs
- Building multi-step AI systems
- Implementing ReAct-style agents
- Tool integration with LLMs
- Designing reasoning-driven workflows

## 🧑‍💻 Author

AI Engineer in training — building intelligent, tool-using agents for real-world problem solving.
