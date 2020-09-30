# Introducción a la programación probabilística

Created By: Robert H C
Last Edited: Sep 29, 2020 10:43 PM
Tags: Data Science, Platzi

La programación probabilística utiliza probabilidades y modelos probabilísticos para ejecutar cómputos, Se utiliza en campos como investigación científica, inteligencia artificial, medicina, etc.

Existen librerías para ejecutar este computo, como Pyro de Uber.

- Las probabilidades cuando de un subconjunto (&) son menos probables

    ![./img/probabilidad.png](./img/probabilidad.png)

    Ejm: Ser musico y consumir drogras es menos probable

## Probabilidad condicional

Cuando tenemos probabilidades condicionales, tenemos que conciderar el evento anterior.

```python
P(A and B) = P(A) . P(B|A)
P(B) = P(A) . P(B|A) + P(~A) . P(B|~A)
```

## Teorema de Bayes

La probabilidad no es directa a una caso, se necesita pensar en las demás exploraciones. Cual es la probabilidad inicial, una vez aplicada las probabilidades directa a una población cual es el resultado posterior. 

```python
					P(B|A) . P(A)
P(A|B) = ---------------
							P(B)

					P(H and E)
P(H|E) = ---------------
							P(E)

```

![./img/teoremabayes.png](./img/teoremabayes.png)

H = hipótesis

E = Evento

P(H) = Prior = hipótesis antes de la evidencia

P(H|E) = Posterior = Ya teniendo evidencia como actualizamos cierta creencia.

P(E|H) = Likelihood = Certeza de que esta situación es correcta.