# MacroSnap 🥑

A minimalist, AI-powered food tracker that estimates calories and macronutrients instantly from a photo to help you reach your nutrition goals with ease.

## Features

- **Instant Food Analysis**: Snap a photo or choose an image from your library to analyze meal composition.
- **Macronutrient Estimation**: Estimates calories, protein, carbs, and fat alongside a detailed ingredients breakdown.
- **Daily Food Log**: Keep track of daily meals with real-time progress towards your calorie and macro targets.
- **Zero-Friction Local Storage**: Persists meals, history, and preferences safely in the browser without requiring external database setups.
- **Flexible AI Integration**:
  - Works out of the box with intelligent nutritional estimation.
  - Supports live **Google Gemini Vision** via `GEMINI_API_KEY` (configured in Vercel or entered directly in the app Profile settings).
  - Supports **OpenAI GPT-4o-mini Vision** via `OPENAI_API_KEY` in Vercel.

## Deploying to Vercel

1. Push this directory to your GitHub / GitLab repository, or deploy directly with the Vercel CLI:
   ```bash
   vercel
   ```
2. (Optional) Set your AI environment variables in your Vercel Project Settings:
   - `GEMINI_API_KEY`: Your Google Gemini API key.
   - `OPENAI_API_KEY`: (Alternative) Your OpenAI API key.
3. Your deployment will be live with SPA rewrites and serverless nutrition analysis at `/api/analyze`.

## Local Testing

You can preview the app locally using any static web server:
```bash
npx serve .
# or
python3 -m http.server 3000
```
Then open `http://localhost:3000` in your browser.
