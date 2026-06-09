# Równania o zmiennych rozdzielonych

## Równania

RoZR 1. $\frac{dy}{dx}=e^{2x+y}$, $y(1)=\ln 2$.

RoZR 2. $xy'+y=y^2$.

RoZR 3. $2x\sqrt{1-y^2}\,dx+y\,dy=0$.

RoZR 4. $x^2(y+1)^3\,dx=(1+x)^3y^3\,dy$.

RoZR 5. $\frac{dy}{dx}=xy^2+x$.

RoZR 6. $(y^2+xy^2)\,dx+(x^2-x^2y)\,dy=0$.

---

## RoZR 1

Założenia: $e^{2x+y}=e^{2x}e^y$, a $e^y\neq 0$ dla każdego $y\in\mathbb{R}$, więc separacja nie pomija żadnych rozwiązań.

Uzasadnienie: równanie ma postać $y'=g(x)h(y)$, gdzie $g(x)=e^{2x}$ oraz $h(y)=e^y$.

Rozdzielenie zmiennych: $e^{-y}\,dy=e^{2x}\,dx$.

Całki: $\int e^{-y}\,dy=\int e^{2x}\,dx$, więc $-e^{-y}=\frac12e^{2x}+C_1$.

Po zmianie stałej: $e^{-y}=C_2-\frac12e^{2x}$.

Warunek początkowy: $y(1)=\ln 2$, więc $e^{-y(1)}=\frac12$.

Podstawienie: $\frac12=C_2-\frac12e^2$, więc $C_2=\frac{1+e^2}{2}$.

Jednoznaczność: $F(x,y)=e^{2x+y}$ oraz $F_y(x,y)=e^{2x+y}$ są ciągłe na obszarze $\{(x,y)\in\mathbb{R}^2\}$. Zatem rozwiązanie jest lokalnie jednoznaczne przez każdy punkt. Dla rozwiązania szczególnego warunek określoności to $\frac{1+e^2-e^{2x}}{2}>0$, czyli $x<\frac12\ln(1+e^2)$.

---

## RoZR 2

Założenia: z równania $xy'+y=y^2$ dostajemy $xy'=y^2-y$. Do postaci normalnej przechodzimy przy $x\neq 0$.

Uzasadnienie: dla $x\neq 0$ mamy $y'=\frac{y^2-y}{x}=\frac1x y(y-1)$, czyli $y'=g(x)h(y)$, gdzie $g(x)=\frac1x$ oraz $h(y)=y(y-1)$.

Przy separacji zakładamy $y\neq 0$ oraz $y\neq 1$, bo dzielimy przez $y(y-1)$.

Sprawdzenie pominiętych warunków: dla $y=0$ mamy $x\cdot 0+0=0^2$, więc $y=0$ jest rozwiązaniem. Dla $y=1$ mamy $x\cdot 0+1=1^2$, więc $y=1$ jest rozwiązaniem.

Rozdzielenie zmiennych: $\frac{dy}{y(y-1)}=\frac{dx}{x}$.

Całki: ponieważ $\frac{1}{y(y-1)}=-\frac1y+\frac1{y-1}$, mamy $\int\frac{dy}{y(y-1)}=\int\frac{dx}{x}$, czyli $-\ln|y|+\ln|y-1|=\ln|x|+C_1$.

Stąd $\ln\left|\frac{y-1}{y}\right|=\ln|x|+C_1$, więc $\frac{y-1}{y}=C_2x$.

Po przekształceniu: $\frac1y=1-C_2x$.

Jednoznaczność: $F(x,y)=\frac{y(y-1)}{x}$ oraz $F_y(x,y)=\frac{2y-1}{x}$ są ciągłe na obszarze $\{(x,y)\in\mathbb{R}^2:x\neq 0\}$. Spójne obszary jednoznaczności to $\{(x,y)\in\mathbb{R}^2:x>0\}$ oraz $\{(x,y)\in\mathbb{R}^2:x<0\}$.

---

## RoZR 3

Założenia: równanie ma sens dla $1-y^2\geq 0$, czyli $-1\leq y\leq 1$.

Po zapisaniu $y=y(x)$: $2x\sqrt{1-y^2}+yy'=0$, więc $yy'=-2x\sqrt{1-y^2}$.

Do separacji zakładamy $-1<y<1$, bo dzielimy przez $\sqrt{1-y^2}$.

Uzasadnienie: dla $-1<y<1$ mamy $\frac{y}{\sqrt{1-y^2}}y'=-2x$, czyli równanie o zmiennych rozdzielonych.

Rozdzielenie zmiennych: $\frac{y}{\sqrt{1-y^2}}\,dy=-2x\,dx$.

Całki: $\int\frac{y}{\sqrt{1-y^2}}\,dy=\int -2x\,dx$.

Po całkowaniu: $-\sqrt{1-y^2}=-x^2+C_1$, więc $\sqrt{1-y^2}=x^2+C_2$, przy czym prawa strona musi być nieujemna.

Sprawdzenie pominiętych warunków: $\sqrt{1-y^2}=0$ daje $y=1$ albo $y=-1$. Obie funkcje stałe spełniają równanie. Przypadek $y=0$ nie daje rozwiązania stałego, bo wtedy zostaje $2x\,dx=0$.

Jednoznaczność: postać normalna to $y'=-\frac{2x\sqrt{1-y^2}}{y}$. Mamy $F(x,y)=-\frac{2x\sqrt{1-y^2}}{y}$ oraz $F_y(x,y)=\frac{2x}{y^2\sqrt{1-y^2}}$. Są ciągłe na obszarze $\{(x,y)\in\mathbb{R}^2:-1<y<1,\ y\neq 0\}$. Spójne obszary jednoznaczności to $\{(x,y)\in\mathbb{R}^2:0<y<1\}$ oraz $\{(x,y)\in\mathbb{R}^2:-1<y<0\}$.

---

## RoZR 4

Założenia: po zapisaniu $y=y(x)$ mamy $x^2(y+1)^3=(1+x)^3y^3y'$. Do postaci normalnej zakładamy $x\neq -1$ oraz $y\neq 0$.

Uzasadnienie: dla $x\neq -1$ i $y\neq 0$ mamy $y'=\frac{x^2(y+1)^3}{(1+x)^3y^3}=\frac{x^2}{(1+x)^3}\cdot\frac{(y+1)^3}{y^3}$, czyli $y'=g(x)h(y)$, gdzie $g(x)=\frac{x^2}{(1+x)^3}$ oraz $h(y)=\frac{(y+1)^3}{y^3}$.

Przy separacji zakładamy dodatkowo $y\neq -1$, bo dzielimy przez $(y+1)^3$.

Rozdzielenie zmiennych: $\frac{y^3}{(y+1)^3}\,dy=\frac{x^2}{(1+x)^3}\,dx$.

Całki: $\int\frac{y^3}{(y+1)^3}\,dy=\int\frac{x^2}{(1+x)^3}\,dx$.

Lewa strona: dla $t=y+1$ mamy $\frac{y^3}{(y+1)^3}=\frac{(t-1)^3}{t^3}=1-\frac3t+\frac3{t^2}-\frac1{t^3}$, więc całka wynosi $(y+1)-3\ln|y+1|-\frac3{y+1}+\frac{1}{2(y+1)^2}$.

Prawa strona: dla $s=x+1$ mamy $\frac{x^2}{(x+1)^3}=\frac{(s-1)^2}{s^3}=\frac1s-\frac2{s^2}+\frac1{s^3}$, więc całka wynosi $\ln|x+1|+\frac2{x+1}-\frac{1}{2(x+1)^2}$.

Sprawdzenie pominiętych warunków: dla $y=-1$ mamy $dy=0$ oraz $(y+1)^3=0$, więc $y=-1$ spełnia równanie. Dla $y=0$ równanie daje $x^2\,dx=0$, więc $y=0$ nie jest rozwiązaniem na przedziale.

Jednoznaczność: $F(x,y)=\frac{x^2(y+1)^3}{(1+x)^3y^3}$. Funkcja $F$ oraz $F_y$ są ciągłe na obszarze $\{(x,y)\in\mathbb{R}^2:x\neq -1,\ y\neq 0\}$. Spójne obszary jednoznaczności to $\{(x,y)\in\mathbb{R}^2:x>-1,\ y>0\}$, $\{(x,y)\in\mathbb{R}^2:x>-1,\ y<0\}$, $\{(x,y)\in\mathbb{R}^2:x<-1,\ y>0\}$ oraz $\{(x,y)\in\mathbb{R}^2:x<-1,\ y<0\}$.

---

## RoZR 5

Założenia: $xy^2+x=x(y^2+1)$, a $y^2+1>0$ dla każdego $y\in\mathbb{R}$. Separacja nie pomija żadnych rozwiązań.

Uzasadnienie: równanie ma postać $y'=x(y^2+1)$, czyli $y'=g(x)h(y)$, gdzie $g(x)=x$ oraz $h(y)=y^2+1$.

Rozdzielenie zmiennych: $\frac{dy}{y^2+1}=x\,dx$.

Całki: $\int\frac{dy}{y^2+1}=\int x\,dx$.

Po całkowaniu: $\arctan y=\frac{x^2}{2}+C$.

Jednoznaczność: $F(x,y)=x(y^2+1)$ oraz $F_y(x,y)=2xy$ są ciągłe na obszarze $\{(x,y)\in\mathbb{R}^2\}$. Zatem równanie ma lokalnie jednoznaczne rozwiązanie przez każdy punkt płaszczyzny. Jawna postać z tangensem obowiązuje na przedziałach, na których $\cos\left(\frac{x^2}{2}+C\right)\neq 0$.

---

## RoZR 6

Założenia: upraszczamy równanie do postaci $y^2(1+x)\,dx+x^2(1-y)\,dy=0$.

Po zapisaniu $y=y(x)$: $y^2(1+x)+x^2(1-y)y'=0$.

Do postaci normalnej zakładamy $x\neq 0$ oraz $y\neq 1$.

Uzasadnienie: wtedy $y'=-\frac{y^2(1+x)}{x^2(1-y)}=-\frac{1+x}{x^2}\cdot\frac{y^2}{1-y}$, czyli $y'=g(x)h(y)$, gdzie $g(x)=-\frac{1+x}{x^2}$ oraz $h(y)=\frac{y^2}{1-y}$.

Przy separacji zakładamy dodatkowo $y\neq 0$, bo dzielimy przez $y^2$.

Rozdzielenie zmiennych: $\frac{1-y}{y^2}\,dy=-\frac{1+x}{x^2}\,dx$.

Całki: $\int\frac{1-y}{y^2}\,dy=\int-\frac{1+x}{x^2}\,dx$.

Lewa strona: $\frac{1-y}{y^2}=\frac1{y^2}-\frac1y$, więc $\int\frac{1-y}{y^2}\,dy=-\frac1y-\ln|y|$.

Prawa strona: $-\frac{1+x}{x^2}=-\frac1{x^2}-\frac1x$, więc $\int-\frac{1+x}{x^2}\,dx=\frac1x-\ln|x|$.

Po całkowaniu: $-\frac1y-\ln|y|=\frac1x-\ln|x|+C$.

Sprawdzenie pominiętych warunków: dla $y=0$ mamy $dy=0$ oraz $y^2=0$, więc $y=0$ spełnia równanie. Dla $y=1$ mamy $dy=0$, ale zostaje $(1+x)\,dx=0$, więc $y=1$ nie jest rozwiązaniem na przedziale.

Jednoznaczność: $F(x,y)=-\frac{y^2(1+x)}{x^2(1-y)}$. Funkcja $F$ oraz $F_y$ są ciągłe na obszarze $\{(x,y)\in\mathbb{R}^2:x\neq 0,\ y\neq 1\}$. Spójne obszary jednoznaczności to $\{(x,y)\in\mathbb{R}^2:x>0,\ y<1\}$, $\{(x,y)\in\mathbb{R}^2:x>0,\ y>1\}$, $\{(x,y)\in\mathbb{R}^2:x<0,\ y<1\}$ oraz $\{(x,y)\in\mathbb{R}^2:x<0,\ y>1\}$.

---

## Odpowiedzi

RoZR 1:

Rozwiązanie ogólne: $y=-\ln\left(C-\frac12e^{2x}\right)$, gdzie $C-\frac12e^{2x}>0$.

Rozwiązanie szczególne: $\boxed{y=-\ln\left(\frac{1+e^2-e^{2x}}{2}\right)}$.

Przedział maksymalny rozwiązania szczególnego: $\boxed{x\in\left(-\infty,\frac12\ln(1+e^2)\right)}$.

RoZR 2:

Rozwiązanie ogólne: $\boxed{y=\frac{1}{1+Cx}}$.

Rozwiązanie szczególne pominięte przy separacji: $\boxed{y=0}$.

Rozwiązanie $y=1$ jest zawarte w rodzinie ogólnej dla $C=0$.

Obszary jednoznaczności: $\boxed{\{(x,y)\in\mathbb{R}^2:x>0\}}$ oraz $\boxed{\{(x,y)\in\mathbb{R}^2:x<0\}}$.

RoZR 3:

Rozwiązanie ogólne: $\boxed{\sqrt{1-y^2}=x^2+C}$, gdzie $0\le x^2+C\le 1$.

W szczególności na odpowiednich przedziałach: $\boxed{y=\pm\sqrt{1-(x^2+C)^2}}$.

Rozwiązania szczególne: $\boxed{y=1}$ oraz $\boxed{y=-1}$.

Obszary jednoznaczności: $\boxed{\{(x,y)\in\mathbb{R}^2:0<y<1\}}$ oraz $\boxed{\{(x,y)\in\mathbb{R}^2:-1<y<0\}}$.

RoZR 4:

Rozwiązanie ogólne:

$$
\boxed{
(y+1)-3\ln|y+1|-\frac3{y+1}+\frac{1}{2(y+1)^2}
=
\ln|x+1|+\frac2{x+1}-\frac{1}{2(x+1)^2}+C
}.
$$

Rozwiązanie szczególne: $\boxed{y=-1}$.

Obszary jednoznaczności: $\boxed{\{(x,y)\in\mathbb{R}^2:x>-1,\ y>0\}}$, $\boxed{\{(x,y)\in\mathbb{R}^2:x>-1,\ y<0\}}$, $\boxed{\{(x,y)\in\mathbb{R}^2:x<-1,\ y>0\}}$, $\boxed{\{(x,y)\in\mathbb{R}^2:x<-1,\ y<0\}}$.

RoZR 5:

Rozwiązanie ogólne: $\boxed{\arctan y=\frac{x^2}{2}+C}$.

Postać jawna: $\boxed{y=\tan\left(\frac{x^2}{2}+C\right)}$ na przedziałach, gdzie $\cos\left(\frac{x^2}{2}+C\right)\neq 0$.

Obszar jednoznaczności: $\boxed{\{(x,y)\in\mathbb{R}^2\}}$.

RoZR 6:

Rozwiązanie ogólne: $\boxed{\frac1y+\ln|y|=-\frac1x+\ln|x|+C}$.

Rozwiązanie szczególne: $\boxed{y=0}$.

Obszary jednoznaczności: $\boxed{\{(x,y)\in\mathbb{R}^2:x>0,\ y<1\}}$, $\boxed{\{(x,y)\in\mathbb{R}^2:x>0,\ y>1\}}$, $\boxed{\{(x,y)\in\mathbb{R}^2:x<0,\ y<1\}}$ oraz $\boxed{\{(x,y)\in\mathbb{R}^2:x<0,\ y>1\}}$.
