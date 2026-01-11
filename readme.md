# Drone Security Analyst Agent (AI Engineer Assignment)

## Overview

This project is a prototype implementation of a **Drone Security Analyst Agent** designed to monitor a fixed property using simulated drone telemetry and video observations.

The system demonstrates how raw drone data can be transformed into **structured, searchable intelligence** and how an AI agent can reason over historical observations to provide **precise, human-readable answers** to security-related questions.

The focus of this prototype is on:
- AI-driven reasoning
- Context management
- Frame-by-frame indexing
- Explainability

rather than raw computer vision accuracy.

---

## Key Capabilities

- **Simulated Real-Time Processing**
  - Sequential ingestion of telemetry (time, location)
  - Processing of simulated video frame descriptions

- **Vision-Language Model (VLM) Abstraction**
  - Video frames are represented as text descriptions
  - Mimics the output of a real VLM (e.g., BLIP / CLIP)
  - Allows easy replacement with real vision models in future

- **Frame-Level Indexing**
  - All observations are stored in a SQLite database
  - Indexed by time, location, description, and object type
  - Enables historical querying and reasoning

- **AI-Powered Analyst Q&A**
  - Natural language questions answered using an LLM
  - Answers are derived strictly from indexed observations
  - Responses are concise, aggregated, and query-aligned

- **Explainable Event Logging**
  - Each detected event is logged clearly with context

---

## Feature Specification

### Value to Property Owners
Enhances property security by providing continuous monitoring, historical visibility, and AI-assisted analysis of drone observations.

### Core Requirements
1. Analyze telemetry and video observations sequentially.
2. Identify and store objects or activities with contextual metadata.
3. Enable querying and reasoning over historical observations.

---

## System Architecture

