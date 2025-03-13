# Benchmarking

```bash
./exec.sh
```


## La série de Leibniz

Calcul de pi, la série de Leibniz : https://fr.wikipedia.org/wiki/Formule_de_Leibniz#S%C3%A9rie_altern%C3%A9e

La série de Leibniz pour l'approximation de \(\pi\) est donnée par :

$\[
\pi = 4 \sum_{k=0}^{\infty} \frac{(-1)^k}{2k+1}
\]$

Ou de manière développée :

$\[
\pi = 4 \left( 1 - \frac{1}{3} + \frac{1}{5} - \frac{1}{7} + \frac{1}{9} - \frac{1}{11} + \dots \right)
\]$

Cette série converge très lentement vers \(\pi\), ce qui la rend peu efficace pour les calculs numériques précis.

## Temps écoulés :

| **Opération** | **Temps écoulé** |
|    ---        |      ---         |
| rust          | 8,3^-5 ms        |
| c             | 3.5 ms           |
| js            | 11.3 ms          |
| python        | 259 ms           |
| Haskell       | 0.132 ms         |
| Julia         | 38 ms            |
