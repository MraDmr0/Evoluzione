# Evoluzione

Classe Python che permette di simulare l'evoluzione temporale di sistemi quantistici a n-livelli soggetti ad un potenziale eletttrico oscillante:

```math
V(t)_{i,j} = -i F cos( \omega t ) \omega^{i,j}_{r} \exp\left(-i( \omega ^ {j}_{l}-\omega^{i}_{l})t\right)
```

Il sistema fisico è determinato dall'energia dei suoi livelli (frequenze di Larmor) e dal suo accoppiamento con il campo elettrico (frequenze di Rabi); il potenziale invece è caratterizato dalla sua frequenza di oscillazione ($\omega$) e dalla sua intensità $F$. L'integrazione temporale dell'equazione di Schrodinger avviene tramite l'algoritmo di Runge-Kutta al quarto ordine.

## Input

* prefix                = (str) nome per output file
* D                     = (int) numero di stati
* ti                    = (float) tempo iniziale in micro sec
* tf                    = (float) tempo finale in micro sec
* N                     = (int) numero di step 
* n                     = (array) condizione iniziale
* wl                    = (array) frequenze di Larmor (meV)
* wr                    = (array) frequenze di Rabi  (Hz)
* w                     = (float) frequenza di oscillazione del campo (Hz)
*F                      = (float) intensità del campo

Mario Di Mare.
