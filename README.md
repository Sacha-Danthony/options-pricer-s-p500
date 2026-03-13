# Options Pricer — S&P500 🇺🇸
Pricing d'options européennes sur le S&P500 en Python — 
Black-Scholes, Monte Carlo, calcul des grecques et 
analyse de la volatilité implicite sur données réelles.

## Concepts couverts
* Black-Scholes : pricing analytique d'options call/put européennes
* Grecques : Delta, Gamma, Vega, Theta, Rho
* Monte Carlo : simulation de 50 000 trajectoires et convergence vers BS
* Parité Call-Put : validation mathématique du pricer
* Volatilité implicite : calcul par inversion numérique de BS (Brentq)
* Smile de volatilité : analyse du skew sur données réelles SPY

## Technologies
* Python 3
* NumPy
* SciPy
* Matplotlib
* yfinance
* Pandas

## Résultats
* Prix Call/Put en fonction du sous-jacent
* Delta en fonction du sous-jacent
* Convergence Monte Carlo vs Black-Scholes
* Grecques (Gamma, Vega, Theta)
* Smile de volatilité implicite — Calls vs Puts (données réelles SPY)

## Paramètres utilisés
 Paramètre  Valeur 

 Sous-jacent : S&P500, Prix actuel (S) : 6740$, Strike (K) : 6740$, Maturité (T) : 1 an, Taux sans risque (r) : 3.75%, Volatilité (σ) : 25%, Données options réelles : SPY via yfinance 

## Conclusions
* BS suppose une volatilité constante — le smile prouve que c'est faux
* Le skew montre que le marché surpaye la protection contre les baisses
* BS sous-estime le risque de queue sur les strikes bas

## Lancer le projet
pip install numpy scipy matplotlib yfinance pandas
jupyter notebook options_pricer.ipynb

## Auteur
Sacha Danthony — Étudiant en Finance INSEEC Bachelor 
