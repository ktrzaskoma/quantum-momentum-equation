# Rozwiązanie
Rozwiązanie jest zawarte na dole pliku **kwanty02a.ipnyb**. Gdyby plik nie wyświetlał się poniżej zamieszczam rozwiązanie:

* Średni pęd w n-tym stanie stacjonarnym:
```python
p1 = sp.integrate(sol.rhs.conjugate() * sol.rhs.diff(x), (x, 0, a)).simplify()
p1
```
* Średni kwadrat pędu w n-tym stanie stacjonarnym:
```python
p2 = -h**2 * sp.integrate(sol.rhs.conjugate() * sol.rhs.diff(x, x), (x, 0, a)).simplify()
p2
```
