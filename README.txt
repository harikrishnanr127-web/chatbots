10 study chatbots (Flask + Gemini, model gemini-3.1-flash-lite)

Each folder is a separate app. To run one:
  cd 01_mathmate
  add your key to .env  ->  GEMINI_API_KEY=...
  pip install -r requirements.txt
  python app.py          (production: gunicorn app:app)

Run several at once by giving each its own port:  PORT=5001 python app.py
If the model ID is rejected, set GEMINI_MODEL=<exact-id> in .env.
