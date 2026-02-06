# MealMind – Smart Daily Meal Planner

MealMind is an AI-powered daily meal planning application built using
Amazon PartyRock and Amazon Bedrock. The project demonstrates how
AWS-managed generative AI services can be used to build a practical,
user-facing application without managing any infrastructure.

This project is aligned with **AWS Cloud Practitioner (CLF-C02)** concepts
such as managed services, service abstraction, shared responsibility,
and cost-aware cloud usage.

---

## Overview

MealMind generates a balanced daily meal plan based on:
- User-defined calorie target
- Dietary preference (vegetarian / non-vegetarian)
- Number of meals per day

The application focuses on **prompt engineering and cloud-native design**
rather than traditional backend development.

---

## Features

- Calorie-based daily meal planning
- Dietary preference handling
- Balanced distribution across meals
- Clean, structured, and readable output
- Fully managed cloud execution (no servers)

---

## Architecture


**Flow (high-level):**
1. User enters inputs in the PartyRock UI
2. PartyRock widgets build a prompt payload (template + inputs)
3. The prompt is sent to the Amazon Bedrock Runtime API
4. Bedrock invokes a foundation model (e.g., Titan, Claude, Llama)
5. Generated output is returned and rendered in the PartyRock app

All infrastructure, scaling, and model hosting are handled by AWS.

---

## AWS Services Used

- **Amazon PartyRock** – No-code UI and workflow orchestration
- **Amazon Bedrock** – Managed foundation model inference
- **Foundation Models** – Invoked via Bedrock (model selection abstracted)

---

## AWS Cloud Practitioner Concepts Demonstrated

- Managed AWS services
- No infrastructure or server management
- Service abstraction (UI layer vs model runtime)
- Shared Responsibility Model
- Cost-aware design using free usage limits

---

## Example

**Input:**
- Daily calories: 2000 kcal  
- Diet preference: Non-vegetarian  
- Meals per day: 3  

**Output:**
- Breakfast, lunch, and dinner with estimated calories
- Total calories kept within target

---



---

## Learnings

- Designing constraint-based prompts for deterministic output
- Understanding the role of managed generative AI services in AWS
- Applying AWS Cloud Practitioner concepts in a real-world use case
- Documenting cloud projects for portfolio presentation

---

## Tags

AWS, Amazon Bedrock, PartyRock, Generative AI, Prompt Engineering,
Cloud Practitioner, Serverless, Portfolio Project
