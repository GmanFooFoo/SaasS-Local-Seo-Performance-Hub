# AI Architecture

## High-Level Architecture
- The AI layer is a core part of the backend, processing data from multiple sources (rankings, reviews, citations).
- AI models are accessed via APIs and microservices.
- Data flows from ingestion → preprocessing → AI analysis → results storage → dashboard/API.

## Technologies & Models
- OpenAI GPT models for text analysis and recommendations
- Custom scoring algorithms for visibility
- Sentiment analysis models for reviews

## Integration Points
- REST API endpoints for triggering AI analysis
- Scheduled jobs for periodic data refresh and scoring