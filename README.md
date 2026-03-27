# NutriPlan — AI Diet & Meal Planner

Get a personalised weekly meal plan with macros, ingredients, prep times, and a shopping list — tailored to your goals and dietary preferences.

## Features
- Goal selection (lose weight, build muscle, maintain, etc.)
- Diet types (omnivore, vegetarian, vegan, keto, paleo, mediterranean)
- Calorie target + allergy configuration
- 1–7 day plans with 2–5 meals per day
- Per-meal macros (protein, carbs, fat) and prep time
- Auto-generated shopping list
- Nutrition tips
- Chat-based nutritionist for follow-up questions

## Stack
- **Frontend**: React 18, Vite, Tailwind CSS v4, Framer Motion
- **Backend**: FastAPI, Groq SDK

## Local Development

### Backend
```bash
cd backend && python -m venv venv && source venv/bin/activate
pip install -r requirements.txt && cp .env.example .env
uvicorn main:app --reload --port 8000
```

### Frontend
```bash
cd frontend && npm install
echo "VITE_API_BASE_URL=http://localhost:8000" > .env
npm run dev
```
