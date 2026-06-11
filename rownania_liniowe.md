# Równania liniowe pierwszego rzędu

## Zadania

### RL 1

Rozwiązać równanie $y'=y\tan x+2\sin x$.

### RL 2

Rozwiązać zagadnienie początkowe $y'-\frac{2x}{1+x^2}y=x^2$, $y(1)=0$.

### RL 3

Rozwiązać równanie $y'+2xy=e^{-x^2}$.

### RL 4

Rozwiązać równanie $y'-2xy=2x^3$.

### RL 5

Rozwiązać równanie $y'+y\cos x=\sin x\cos x$.

### RL 6

Rozwiązać równanie $y'-e^xy=e^{2x}$.

### RL 7

Rozwiązać zagadnienie początkowe $y'+\frac{1-2x}{x^2}y=1$, $y(1)=1+e$.

---

## Rozwiązania

### RL 1

Równanie: $y'=y\tan x+2\sin x$.

Postać liniowa $y'+p(x)y=q(x)$: $y'-(\tan x)y=2\sin x$.

Założenia: $\cos x\neq 0$.

Równanie jednorodne: $y'-(\tan x)y=0$.

Rozwiązanie równania jednorodnego: $\frac{dy}{y}=\tan x\,dx$, więc $\ln|y|=-\ln|\cos x|+C$ i $y=\frac{C}{\cos x}$.

Uzmiennianie stałej: $y=\frac{C(x)}{\cos x}$.

Podstawienie do równania: $y'=\frac{C'(x)}{\cos x}+\frac{C(x)\sin x}{\cos^2 x}$, zatem
$\frac{C'(x)}{\cos x}+\frac{C(x)\sin x}{\cos^2 x}-\frac{C(x)}{\cos x}\tan x=2\sin x$.

Wyznaczenie $C'(x)$: $\frac{C'(x)}{\cos x}=2\sin x$, więc $C'(x)=2\sin x\cos x$.

Całkowanie: $C(x)=\sin^2 x+C_1$.

Rozwiązanie ogólne: $y=\frac{\sin^2 x+C}{\cos x}$.

Wynik końcowy: $\boxed{y=\frac{\sin^2 x+C}{\cos x}}$ na przedziałach, na których $\cos x\neq 0$.

---

### RL 2

Równanie: $y'-\frac{2x}{1+x^2}y=x^2$, $y(1)=0$.

Postać liniowa $y'+p(x)y=q(x)$: $y'-\frac{2x}{1+x^2}y=x^2$.

Założenia: brak.

Równanie jednorodne: $y'-\frac{2x}{1+x^2}y=0$.

Rozwiązanie równania jednorodnego: $\frac{dy}{y}=\frac{2x}{1+x^2}\,dx$, więc $\ln|y|=\ln(1+x^2)+C$ i $y=C(1+x^2)$.

Uzmiennianie stałej: $y=C(x)(1+x^2)$.

Podstawienie do równania: $y'=C'(x)(1+x^2)+2xC(x)$, zatem
$C'(x)(1+x^2)+2xC(x)-\frac{2x}{1+x^2}C(x)(1+x^2)=x^2$.

Wyznaczenie $C'(x)$: $C'(x)(1+x^2)=x^2$, więc $C'(x)=\frac{x^2}{1+x^2}=1-\frac{1}{1+x^2}$.

Całkowanie: $C(x)=x-\arctan x+C_1$.

Rozwiązanie ogólne: $y=(1+x^2)(x-\arctan x+C_1)$.

Warunek początkowy: $0=y(1)=2\left(1-\frac{\pi}{4}+C_1\right)$, więc $C_1=\frac{\pi}{4}-1$.

Przedział jednoznaczności: ponieważ $F(x,y)=\frac{2x}{1+x^2}y+x^2$ oraz $F_y(x,y)=\frac{2x}{1+x^2}$ są ciągłe na $\mathbb{R}^2$, rozwiązanie jest jednoznaczne dla $x\in\mathbb{R}$.

Wynik końcowy: $\boxed{y=(1+x^2)\left(x-\arctan x+\frac{\pi}{4}-1\right)}$, $x\in\mathbb{R}$.

---

### RL 3

Równanie: $y'+2xy=e^{-x^2}$.

Postać liniowa $y'+p(x)y=q(x)$: $y'+2xy=e^{-x^2}$.

Założenia: brak.

Równanie jednorodne: $y'+2xy=0$.

Rozwiązanie równania jednorodnego: $\frac{dy}{y}=-2x\,dx$, więc $\ln|y|=-x^2+C$ i $y=Ce^{-x^2}$.

Uzmiennianie stałej: $y=C(x)e^{-x^2}$.

Podstawienie do równania: $y'=C'(x)e^{-x^2}-2xC(x)e^{-x^2}$, zatem
$C'(x)e^{-x^2}-2xC(x)e^{-x^2}+2xC(x)e^{-x^2}=e^{-x^2}$.

Wyznaczenie $C'(x)$: $C'(x)e^{-x^2}=e^{-x^2}$, więc $C'(x)=1$.

Całkowanie: $C(x)=x+C_1$.

Rozwiązanie ogólne: $y=(x+C)e^{-x^2}$.

Wynik końcowy: $\boxed{y=(x+C)e^{-x^2}}$.

---

### RL 4

Równanie: $y'-2xy=2x^3$.

Postać liniowa $y'+p(x)y=q(x)$: $y'-2xy=2x^3$.

Założenia: brak.

Równanie jednorodne: $y'-2xy=0$.

Rozwiązanie równania jednorodnego: $\frac{dy}{y}=2x\,dx$, więc $\ln|y|=x^2+C$ i $y=Ce^{x^2}$.

Uzmiennianie stałej: $y=C(x)e^{x^2}$.

Podstawienie do równania: $y'=C'(x)e^{x^2}+2xC(x)e^{x^2}$, zatem
$C'(x)e^{x^2}+2xC(x)e^{x^2}-2xC(x)e^{x^2}=2x^3$.

Wyznaczenie $C'(x)$: $C'(x)e^{x^2}=2x^3$, więc $C'(x)=2x^3e^{-x^2}$.

Całkowanie: $C(x)=\int 2x^3e^{-x^2}\,dx=-(x^2+1)e^{-x^2}+C_1$.

Rozwiązanie ogólne: $y=\left(-(x^2+1)e^{-x^2}+C_1\right)e^{x^2}=Ce^{x^2}-x^2-1$.

Wynik końcowy: $\boxed{y=Ce^{x^2}-x^2-1}$.

---

### RL 5

Równanie: $y'+y\cos x=\sin x\cos x$.

Postać liniowa $y'+p(x)y=q(x)$: $y'+(\cos x)y=\sin x\cos x$.

Założenia: brak.

Równanie jednorodne: $y'+y\cos x=0$.

Rozwiązanie równania jednorodnego: $\frac{dy}{y}=-\cos x\,dx$, więc $\ln|y|=-\sin x+C$ i $y=Ce^{-\sin x}$.

Uzmiennianie stałej: $y=C(x)e^{-\sin x}$.

Podstawienie do równania: $y'=C'(x)e^{-\sin x}-C(x)\cos x\,e^{-\sin x}$, zatem
$C'(x)e^{-\sin x}-C(x)\cos x\,e^{-\sin x}+C(x)e^{-\sin x}\cos x=\sin x\cos x$.

Wyznaczenie $C'(x)$: $C'(x)e^{-\sin x}=\sin x\cos x$, więc $C'(x)=e^{\sin x}\sin x\cos x$.

Całkowanie: $C(x)=\int e^{\sin x}\sin x\cos x\,dx=(\sin x-1)e^{\sin x}+C_1$.

Rozwiązanie ogólne: $y=\left((\sin x-1)e^{\sin x}+C_1\right)e^{-\sin x}=\sin x-1+Ce^{-\sin x}$.

Wynik końcowy: $\boxed{y=\sin x-1+Ce^{-\sin x}}$.

---

### RL 6

Równanie: $y'-e^xy=e^{2x}$.

Postać liniowa $y'+p(x)y=q(x)$: $y'-(e^x)y=e^{2x}$.

Założenia: brak.

Równanie jednorodne: $y'-e^xy=0$.

Rozwiązanie równania jednorodnego: $\frac{dy}{y}=e^x\,dx$, więc $\ln|y|=e^x+C$ i $y=Ce^{e^x}$.

Uzmiennianie stałej: $y=C(x)e^{e^x}$.

Podstawienie do równania: $y'=C'(x)e^{e^x}+C(x)e^{e^x}e^x$, zatem
$C'(x)e^{e^x}+C(x)e^{e^x}e^x-e^xC(x)e^{e^x}=e^{2x}$.

Wyznaczenie $C'(x)$: $C'(x)e^{e^x}=e^{2x}$, więc $C'(x)=e^{2x-e^x}$.

Całkowanie: $C(x)=\int e^{2x-e^x}\,dx=-(e^x+1)e^{-e^x}+C_1$.

Rozwiązanie ogólne: $y=\left(-(e^x+1)e^{-e^x}+C_1\right)e^{e^x}=Ce^{e^x}-e^x-1$.

Wynik końcowy: $\boxed{y=Ce^{e^x}-e^x-1}$.

---

### RL 7

Równanie: $y'+\frac{1-2x}{x^2}y=1$, $y(1)=1+e$.

Postać liniowa $y'+p(x)y=q(x)$: $y'+\frac{1-2x}{x^2}y=1$.

Założenia: $x\neq 0$.

Równanie jednorodne: $y'+\frac{1-2x}{x^2}y=0$.

Rozwiązanie równania jednorodnego: $\frac{dy}{y}=-\frac{1-2x}{x^2}\,dx=\left(-\frac{1}{x^2}+\frac{2}{x}\right)\,dx$, więc $\ln|y|=\frac{1}{x}+2\ln|x|+C$ i $y=Cx^2e^{1/x}$.

Uzmiennianie stałej: $y=C(x)x^2e^{1/x}$.

Podstawienie do równania: $y'=C'(x)x^2e^{1/x}+C(x)e^{1/x}(2x-1)$, zatem
$C'(x)x^2e^{1/x}+C(x)e^{1/x}(2x-1)+\frac{1-2x}{x^2}C(x)x^2e^{1/x}=1$.

Wyznaczenie $C'(x)$: $C'(x)x^2e^{1/x}=1$, więc $C'(x)=\frac{e^{-1/x}}{x^2}$.

Całkowanie: $C(x)=e^{-1/x}+C_1$.

Rozwiązanie ogólne: $y=x^2+C_1x^2e^{1/x}$.

Warunek początkowy: $1+e=y(1)=1+C_1e$, więc $C_1=1$.

Przedział jednoznaczności: $F(x,y)=1-\frac{1-2x}{x^2}y$ oraz $F_y(x,y)=-\frac{1-2x}{x^2}$ są ciągłe dla $x\neq 0$. Ponieważ punkt początkowy ma $x=1$, bierzemy przedział $(0,\infty)$.

Wynik końcowy: $\boxed{y=x^2+x^2e^{1/x}}$, $x\in(0,\infty)$.

---

## Odpowiedzi

RL 1. $\boxed{y=\frac{\sin^2 x+C}{\cos x}}$, na przedziałach, na których $\cos x\neq 0$.

RL 2. $\boxed{y=(1+x^2)\left(x-\arctan x+\frac{\pi}{4}-1\right)}$, $x\in\mathbb{R}$.

RL 3. $\boxed{y=(x+C)e^{-x^2}}$.

RL 4. $\boxed{y=Ce^{x^2}-x^2-1}$.

RL 5. $\boxed{y=\sin x-1+Ce^{-\sin x}}$.

RL 6. $\boxed{y=Ce^{e^x}-e^x-1}$.

RL 7. $\boxed{y=x^2+x^2e^{1/x}}$, $x\in(0,\infty)$.
