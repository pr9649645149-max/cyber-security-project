# PhishGuard

A simple anti-phishing email risk analyzer.

## Features
- Checks sender format
- Detects urgent and suspicious language
- Detects credential-related prompts
- Looks for links and external domains
- Returns a risk score and reasons

## Run locally
1. Create a virtual environment:
   python -m venv .venv
   source .venv/bin/activate

2. Install dependencies:
   pip install -r requirements.txt

3. Start the API:
   uvicorn app.main:app --reload

4. Test the endpoint:
   curl -X POST http://127.0.0.1:8000/analyze \
     -H "Content-Type: application/json" \
     -d '{
       "sender":"support@banksecure-login.com",
       "subject":"Urgent security alert",
       "body":"Your account has been suspended. Verify immediately: http://tinyurl.com/abcd",
       "domain":"banksecure-login.com"
     }'
