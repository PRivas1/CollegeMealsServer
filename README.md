# CollegeMeals Server 

A lightweight Node.js/Express server that acts as a secure proxy to query Google's Gemini API for meal generation.

##  Purpose

This server hides the Gemini API key from the client by handling the request server-side. It powers the [CollegeMeals App](https://collegemeals.app) frontend.

##  Tech Stack

- Node.js
- Express.js
- Hosted on [Render](https://render.com/)

## Why a Server?

- Keeps the Gemini API key safe
- Prevents direct access from frontend clients
- Helps avoid API abuse and quota exhaustion

## How It Works

1. Receives a POST request with a list of ingredients
2. Builds a Gemini prompt and sends it to the API
3. Returns a recipe including prep time and cook time
