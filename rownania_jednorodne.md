# Równania jednorodne względem $x$ i $y$

## Zadania

### RJ 1

Rozwiązać równanie $y'=\frac{x^2+y^2}{xy}$.

### RJ 2

Rozwiązać równanie $y'=\frac{x+y}{3x-y}$.

### RJ 3

Rozwiązać zagadnienie początkowe $y^2+x^2y'=xyy'$, $y(1)=2$.

### RJ 4

Rozwiązać równanie $(y^2-3x^2)\,dy+2xy\,dx=0$.

### RJ 5

Rozwiązać równanie $y-xy'=x+yy'$.

### RJ 6

Rozwiązać równanie $(x^2+2xy-y^2)+(y^2+2xy-x^2)y'=0$.

---

## Rozwiązania

### RJ 1

Równanie: $y'=\frac{x^2+y^2}{xy}$.

Założenia: $x\neq 0$, $y\neq 0$.

Sprowadzamy prawą stronę do funkcji zmiennej $\frac{y}{x}$: $\frac{x^2+y^2}{xy}=\frac{x}{y}+\frac{y}{x}=\frac{1}{y/x}+\frac{y}{x}$.

Podstawiamy $u=\frac{y}{x}$, czyli $y=ux$, $y'=u'x+u$.

Po podstawieniu: $u'x+u=u+\frac{1}{u}$.

Stąd: $xu'=\frac{1}{u}$.

Przy dzieleniu przez $u$ nie powstaje rozwiązanie pominięte, bo $u=0$ odpowiadałoby $y=0$, a dla $y=0$ równanie nie jest określone.

Rozdzielamy zmienne: $u\,du=\frac{dx}{x}$.

Całkujemy: $\frac{u^2}{2}=\ln|x|+C$.

Stąd: $u^2=2\ln|x|+C_1$.

Wracamy do zmiennych $x,y$: $\left(\frac{y}{x}\right)^2=2\ln|x|+C_1$.

Wynik końcowy: $\boxed{y^2=x^2(2\ln|x|+C)}$.

---

### RJ 2

Równanie: $y'=\frac{x+y}{3x-y}$.

Założenia: $x\neq 0$, $3x-y\neq 0$.

Sprowadzamy prawą stronę do funkcji zmiennej $\frac{y}{x}$: $\frac{x+y}{3x-y}=\frac{1+y/x}{3-y/x}$.

Podstawiamy $u=\frac{y}{x}$, czyli $y=ux$, $y'=u'x+u$.

Po podstawieniu: $u'x+u=\frac{1+u}{3-u}$.

Stąd: $xu'=\frac{1+u}{3-u}-u=\frac{(u-1)^2}{3-u}$.

Dla $u\neq 1$ rozdzielamy zmienne: $\frac{3-u}{(u-1)^2}\,du=\frac{dx}{x}$.

Całkujemy: $-\frac{2}{u-1}-\ln|u-1|=\ln|x|+C$.

Po uporządkowaniu: $\frac{2}{u-1}+\ln|x(u-1)|=C_1$.

Wracamy do zmiennych $x,y$: $\frac{2x}{y-x}+\ln|y-x|=C_1$.

Rozwiązanie pominięte przy dzieleniu przez $(u-1)^2$: $u=1$, czyli $y=x$.

Sprawdzenie: dla $y=x$ mamy $y'=1$ oraz $\frac{x+y}{3x-y}=\frac{2x}{2x}=1$.

Wynik końcowy: $\boxed{\frac{2x}{y-x}+\ln|y-x|=C}$ oraz $\boxed{y=x}$.

---

### RJ 3

Równanie: $y^2+x^2y'=xyy'$, $y(1)=2$.

Przekształcamy równanie: $y^2=x(y-x)y'$.

Założenia dla postaci normalnej: $x\neq 0$, $y\neq x$.

Postać normalna: $y'=\frac{y^2}{x(y-x)}$.

Sprowadzamy prawą stronę do funkcji zmiennej $\frac{y}{x}$: $\frac{y^2}{x(y-x)}=\frac{(y/x)^2}{y/x-1}$.

Podstawiamy $u=\frac{y}{x}$, czyli $y=ux$, $y'=u'x+u$.

Po podstawieniu: $u'x+u=\frac{u^2}{u-1}$.

Stąd: $xu'=\frac{u}{u-1}$.

Przy separacji zakładamy dodatkowo $u\neq 0$, czyli $y\neq 0$.

Rozdzielamy zmienne: $\frac{u-1}{u}\,du=\frac{dx}{x}$.

Całkujemy: $u-\ln|u|=\ln|x|+C$.

Wracamy do zmiennych $x,y$: $\frac{y}{x}-\ln|y|=C$.

Rozwiązanie pominięte przy dzieleniu przez $y$: $y=0$.

Sprawdzenie: dla $y=0$ mamy $0+x^2\cdot 0=0$, więc $y=0$ jest rozwiązaniem równania.

Warunek początkowy: $y(1)=2$.

Podstawiamy do rozwiązania ogólnego: $2-\ln 2=C$.

Rozwiązanie szczególne: $\frac{y}{x}-\ln y=2-\ln 2$.

Jednoznaczność: $F(x,y)=\frac{y^2}{x(y-x)}$. Funkcje $F$ oraz $F_y$ są ciągłe na obszarze $\{(x,y)\in\mathbb{R}^2:x>0,\ y>x\}$. Punkt początkowy $(1,2)$ należy do tego obszaru.

Przedział jednoznaczności rozwiązania szczególnego: $x\in\left(\frac{2}{e},\infty\right)$.

Wynik końcowy: $\boxed{\frac{y}{x}-\ln y=2-\ln 2}$, $x\in\left(\frac{2}{e},\infty\right)$.

---

### RJ 4

Równanie: $(y^2-3x^2)\,dy+2xy\,dx=0$.

Zapisujemy w postaci z pochodną: $(y^2-3x^2)y'+2xy=0$.

Założenia: $x\neq 0$. W postaci normalnej dodatkowo $y^2-3x^2\neq 0$.

Mamy: $y'=-\frac{2xy}{y^2-3x^2}$.

Sprowadzamy prawą stronę do funkcji zmiennej $\frac{y}{x}$: $-\frac{2xy}{y^2-3x^2}=-\frac{2(y/x)}{(y/x)^2-3}$.

Podstawiamy $u=\frac{y}{x}$, czyli $y=ux$, $y'=u'x+u$.

Po podstawieniu: $u'x+u=-\frac{2u}{u^2-3}$.

Stąd: $xu'=-\frac{u(u^2-1)}{u^2-3}$.

Dla $u\neq 0$ oraz $u^2\neq 1$ rozdzielamy zmienne: $\frac{3-u^2}{u(u^2-1)}\,du=\frac{dx}{x}$.

Rozkład: $\frac{3-u^2}{u(u^2-1)}=-\frac{3}{u}+\frac{1}{u-1}+\frac{1}{u+1}$.

Całkujemy: $-3\ln|u|+\ln|u-1|+\ln|u+1|=\ln|x|+C$.

Stąd: $\ln\left|\frac{u^2-1}{u^3}\right|=\ln|x|+C$.

Po opuszczeniu logarytmu: $\frac{u^2-1}{u^3}=Cx$.

Wracamy do zmiennych $x,y$: $\frac{y^2-x^2}{y^3}=C$.

Czyli: $y^2-x^2=Cy^3$.

Rozwiązanie pominięte przy dzieleniu przez $u$: $y=0$.

Sprawdzenie: dla $y=0$ mamy $dy=0$ oraz $2xy\,dx=0$, więc równanie jest spełnione.

Rozwiązania $u=1$ i $u=-1$, czyli $y=x$ oraz $y=-x$, są zawarte w rodzinie $y^2-x^2=Cy^3$ dla $C=0$.

Wynik końcowy: $\boxed{y^2-x^2=Cy^3}$ oraz $\boxed{y=0}$.

---

### RJ 5

Równanie: $y-xy'=x+yy'$.

Przekształcamy: $(x+y)y'=y-x$.

Założenia: $x\neq 0$, $x+y\neq 0$.

Mamy: $y'=\frac{y-x}{x+y}$.

Sprowadzamy prawą stronę do funkcji zmiennej $\frac{y}{x}$: $\frac{y-x}{x+y}=\frac{y/x-1}{1+y/x}$.

Podstawiamy $u=\frac{y}{x}$, czyli $y=ux$, $y'=u'x+u$.

Po podstawieniu: $u'x+u=\frac{u-1}{1+u}$.

Stąd: $xu'=-\frac{u^2+1}{u+1}$.

Rozdzielamy zmienne: $\frac{u+1}{u^2+1}\,du=-\frac{dx}{x}$.

Całkujemy: $\frac12\ln(u^2+1)+\arctan u=-\ln|x|+C$.

Po uporządkowaniu: $\ln|x|+\frac12\ln(u^2+1)+\arctan u=C$.

Wracamy do zmiennych $x,y$: $\frac12\ln(x^2+y^2)+\arctan\frac{y}{x}=C$.

Wynik końcowy: $\boxed{\frac12\ln(x^2+y^2)+\arctan\frac{y}{x}=C}$.

---

### RJ 6

Równanie: $(x^2+2xy-y^2)+(y^2+2xy-x^2)y'=0$.

Założenia: $x\neq 0$. W postaci normalnej dodatkowo $y^2+2xy-x^2\neq 0$.

Mamy: $y'=-\frac{x^2+2xy-y^2}{y^2+2xy-x^2}$.

Sprowadzamy prawą stronę do funkcji zmiennej $\frac{y}{x}$: $-\frac{x^2+2xy-y^2}{y^2+2xy-x^2}=-\frac{1+2(y/x)-(y/x)^2}{(y/x)^2+2(y/x)-1}$.

Podstawiamy $u=\frac{y}{x}$, czyli $y=ux$, $y'=u'x+u$.

Po podstawieniu: $u'x+u=-\frac{1+2u-u^2}{u^2+2u-1}$.

Stąd: $xu'=-\frac{(u+1)(u^2+1)}{u^2+2u-1}$.

Dla $u\neq -1$ rozdzielamy zmienne: $-\frac{u^2+2u-1}{(u+1)(u^2+1)}\,du=\frac{dx}{x}$.

Rozkład: $-\frac{u^2+2u-1}{(u+1)(u^2+1)}=-\frac{2u}{u^2+1}+\frac{1}{u+1}$.

Całkujemy: $-\ln(u^2+1)+\ln|u+1|=\ln|x|+C$.

Stąd: $\frac{u+1}{u^2+1}=Cx$.

Wracamy do zmiennych $x,y$: $\frac{x+y}{x^2+y^2}=C$.

Rozwiązanie $u=-1$, czyli $y=-x$, jest zawarte w rodzinie dla $C=0$.

Wynik końcowy: $\boxed{\frac{x+y}{x^2+y^2}=C}$.

---

## Odpowiedzi

RJ 1. $\boxed{y^2=x^2(2\ln|x|+C)}$.

RJ 2. $\boxed{\frac{2x}{y-x}+\ln|y-x|=C}$ oraz $\boxed{y=x}$.

RJ 3. $\boxed{\frac{y}{x}-\ln y=2-\ln 2}$, $x\in\left(\frac{2}{e},\infty\right)$.

RJ 4. $\boxed{y^2-x^2=Cy^3}$ oraz $\boxed{y=0}$.

RJ 5. $\boxed{\frac12\ln(x^2+y^2)+\arctan\frac{y}{x}=C}$.

RJ 6. $\boxed{\frac{x+y}{x^2+y^2}=C}$.
