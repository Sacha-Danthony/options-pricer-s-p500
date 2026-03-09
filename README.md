# Options Pricer — S&P500 🇺🇸

Pricing d'options européennes sur le S&P500 en Python — comparaison Black-Scholes vs Monte Carlo, calcul des grecques et analyse de sensibilité.


## Concepts couverts

- Black-Scholes : pricing analytique d'options call/put européennes
- Grecques : Delta, Gamma, Vega, Theta, Rho
- Monte Carlo : simulation de 50 000 trajectoires et convergence vers B&S
- Parité Call-Put: validation mathématique du pricer


##  Technologies

- Python 3
- NumPy
- SciPy
- Matplotlib


## Résultats

### Prix Call/Put en fonction du sous-jacent
![call_put](images/call_put.png)

### Delta en fonction du sous-jacent
![delta](images/delta.png)

### Convergence Monte Carlo vs Black-Scholes
![convergence](images/convergence.png)

### Grecques (Gamma, Vega, Theta)
![greeks](images/greeks.png)



## Paramètres utilisés

 Paramètre  Valeur 

 Sous-jacent : S&P500 
 Prix actuel (S) : 6740$ 
 Strike (K) : 6740$ 
 Maturité (T) : 1 an 
 Taux sans risque (r) : 3.75% 
 Volatilité (σ) : 25% 

---

## Lancer le projet
```bash
pip install numpy scipy matplotlib
jupyter notebook options_pricer.ipynb
```


## Auteur

[Sacha Danthony] — Étudiant en Finance INSEEC Bachelor 3
