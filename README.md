# ews-bet-date — exporturi pentru dashboard-ul EWS BET

Acest repository public conține CSV-urile citite de aplicația `AnaMerecioni/ews-bet-dashboard`. Fișierele din repository pot fi date demonstrative; înlocuiește-le cu exporturile proaspete din notebook înainte de a prezenta rezultate drept performanță reală a modelului.

## Actualizare după o rulare Kaggle

Descarcă din output-ul notebook-ului și înlocuiește fișierele omonime:

- `predictions.csv` — `Date,stress_probability_20d,stress_threshold,high_threshold,asset`
- `drivers.csv` — `Date,feature,category,contribution,asset`
- `outcomes.csv` — `Date,stress_event_20d,BET,asset`
- `sensitivity.csv` — `feature,shift_sigma,probability`

Nu încărca `train.csv`, `test.csv` sau documentele NLP / datele brute ale competiției.

## Conectare în dashboard

În aplicația EWS BET, deschide pagina **Date** și adaugă linkurile raw:

- https://raw.githubusercontent.com/AnaMerecioni/ews-bet-date/main/predictions.csv
- https://raw.githubusercontent.com/AnaMerecioni/ews-bet-date/main/drivers.csv
- https://raw.githubusercontent.com/AnaMerecioni/ews-bet-date/main/outcomes.csv
- https://raw.githubusercontent.com/AnaMerecioni/ews-bet-date/main/sensitivity.csv

Aplicația citește CSV-urile în browser. GitHub Pages găzduiește doar interfața; antrenarea și generarea datelor se fac în notebook-ul Kaggle.
