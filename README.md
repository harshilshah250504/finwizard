# FinWizard

Stock-price experiments using Yahoo Finance data, news sentiment, and LSTM, CNN, and RNN models.

## Status and prerequisites

This notebook contains successive experiments, with repeated function definitions and historical date windows. Run and review individual experiments separately. Requires internet access for market data and a News API key for the news experiment. Update historical date windows before rerunning. Model results have not been independently reproduced; no accuracy or investment-performance claim is made.

Saved outputs and notebook session metadata have been removed. Dependencies are inferred from imports; a fully reproduced environment and pinned versions are pending.

## Setup

```sh
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter lab notebooks/finwizard.ipynb
```

For the news experiment, set `NEWS_API_KEY` in your environment before starting Jupyter. `.env.example` documents the setting; this notebook does not automatically load `.env` files. Never commit a real API key.

## Author

Harshil Prashant Shah · [Portfolio](https://harshil-prashant-shah.vercel.app/) · [LinkedIn](https://www.linkedin.com/in/harshilpshah/)
