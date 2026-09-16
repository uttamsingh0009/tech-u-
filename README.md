# Tech U — Netlify AI Website

A deployable Tech U website with a Netlify serverless backend connected to the OpenAI Responses API. The OpenAI key stays server-side in Netlify environment variables.

## Netlify
1. Upload this project to a Git repository and import it into Netlify, or deploy the folder with Netlify's deploy flow.
2. In Netlify: Site configuration → Environment variables, add `OPENAI_API_KEY` with your own OpenAI API key.
3. Optional: set `OPENAI_MODEL` to `gpt-5.6-luna` (default).
4. Redeploy after adding the variable.

The frontend calls `/.netlify/functions/chat`; the API key is never placed in browser JavaScript.
