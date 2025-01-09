# Generative-AI-Personalized-Real-State-Agent

## Overview
HomeMatch is an innovative real estate application designed to revolutionize the property search process by tailoring property listings to each buyer's unique preferences. Using Large Language Models (LLMs) and Vector Databases, the application transforms standard real estate listings into personalized narratives, making the home-buying experience more engaging and tailored to individual needs.

## Features
### Buyer Preferences Parsing:

Collect buyer preferences through natural language or structured questions.

Interpret and structure preferences for semantic searches.
### Personalized Listings:

Use LLMs to rewrite property descriptions, emphasizing features that align with buyer preferences.

Ensure factual integrity while tailoring descriptions.
### Semantic Search:

Store real estate listings in a vector database.

Perform semantic searches to retrieve listings that closely match buyer requirements.
### Real Estate Listings Management:

Generate and store synthetic real estate listings using LLMs.

Include detailed property descriptions and neighborhood information.

## Prerequisites
Python 3.9+
Virtual environment tool (e.g., venv or conda)
Required libraries in requirements.txt, including:
LangChain
OpenAI
ChromaDB or LanceDB
pandas
numpy

## Workflow:
### Step 1: Generate Real Estate Listings
Use the provided LLM prompts to create synthetic real estate listings.

Save the listings in data/listings.json or another structured file.
### Step 2: Store Listings in a Vector Database
Configure and initialize a vector database (e.g., ChromaDB).

Convert listings into vector embeddings and store them in the database.
### Step 3: Collect Buyer Preferences
Collect preferences interactively or through hard-coded examples.

Parse and structure preferences for use in semantic search queries.
### Step 4: Perform Semantic Search
Retrieve listings from the vector database that match buyer preferences.

Use a similarity metric to rank and select the most relevant listings.
### Step 5: Personalize Listings
Use LLMs to rewrite the retrieved listings.

Emphasize features that align with buyer preferences while maintaining factual accuracy.

## Example Outputs
### Input Preferences:
I’m looking for a three-bedroom house with eco-friendly features and proximity to public transport.
### Personalized Listing:
This charming three-bedroom home in Green Oaks features solar panels, hardwood floors, and a spacious open kitchen. Conveniently located near Green Oaks Park and public transport, this home is perfect for eco-conscious buyers seeking a blend of comfort and sustainability.
