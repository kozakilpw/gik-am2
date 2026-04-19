# Całki podwójne

## Obliczanie całek podwójnych

**Zadanie 1.**  
Obliczyć całkę podwójną $\iint_D 2y\,dx\,dy$, gdzie $D$ jest obszarem ograniczonym krzywymi: $xy=6$, $x+y=7$.

**Odpowiedź.**  
Punkty przecięcia spełniają układ $xy=6$, $x+y=7$, więc $x(7-x)=6$, czyli $x^2-7x+6=0$. Stąd $x=1$ lub $x=6$, a odpowiednio $y=6$ lub $y=1$.  
Zatem $D=\{(x,y): 1\le x\le 6,\ \frac{6}{x}\le y\le 7-x\}$.  
$\iint_D 2y\,dx\,dy=\int_1^6 \int_{6/x}^{7-x} 2y\,dy\,dx=\int_1^6 \left((7-x)^2-\frac{36}{x^2}\right)\,dx=\frac{125}{3}$.

## Zamiana całki podwójnej na całki iterowane

**Zadanie 2.**  
Na dwa sposoby zamienić całkę podwójną $\iint_D f(x,y)\,dx\,dy$ na całki iterowane, jeżeli $D$ jest obszarem ograniczonym krzywymi: $y=x^2$, $y-x=2$.

**Odpowiedź.**  
Punkty przecięcia spełniają równanie $x^2=x+2$, więc $x=-1$ lub $x=2$.  
Pierwsza postać: $\iint_D f(x,y)\,dx\,dy=\int_{-1}^2 \int_{x^2}^{x+2} f(x,y)\,dy\,dx$.  
Druga postać: $\iint_D f(x,y)\,dx\,dy=\int_0^1 \int_{-\sqrt{y}}^{\sqrt{y}} f(x,y)\,dx\,dy+\int_1^4 \int_{y-2}^{\sqrt{y}} f(x,y)\,dx\,dy$.

**Zadanie 3.**  
Na dwa sposoby zamienić całkę podwójną $\iint_D f(x,y)\,dx\,dy$ na całki iterowane, jeżeli $D$ jest obszarem ograniczonym krzywymi: $x=-1$, $x=1$, $y=|x|$, $y=-\sqrt{4-x^2}$.

**Odpowiedź.**  
Pierwsza postać: $\iint_D f(x,y)\,dx\,dy=\int_{-1}^1 \int_{-\sqrt{4-x^2}}^{|x|} f(x,y)\,dy\,dx$.  
Druga postać:  
$\iint_D f(x,y)\,dx\,dy=\int_{-2}^{-\sqrt{3}} \int_{-\sqrt{4-y^2}}^{\sqrt{4-y^2}} f(x,y)\,dx\,dy+\int_{-\sqrt{3}}^0 \int_{-1}^1 f(x,y)\,dx\,dy$  
$\qquad\qquad\qquad\qquad\qquad\qquad+\int_0^1 \int_{-1}^{-y} f(x,y)\,dx\,dy+\int_0^1 \int_y^1 f(x,y)\,dx\,dy$.

## Zmiana kolejności całkowania

**Zadanie 4.**  
Zmienić kolejność całkowania w podanej całce, a następnie policzyć ją: $\int_1^4 \int_x^{2x} \frac{x}{y^2}\,dy\,dx$.

**Odpowiedź.**  
Obszar całkowania ma opis $1\le x\le 4$, $x\le y\le 2x$.  
Po zmianie kolejności całkowania otrzymujemy  
$\int_1^4 \int_x^{2x} \frac{x}{y^2}\,dy\,dx=\int_1^2 \int_1^y \frac{x}{y^2}\,dx\,dy+\int_2^4 \int_{y/2}^y \frac{x}{y^2}\,dx\,dy+\int_4^8 \int_{y/2}^4 \frac{x}{y^2}\,dx\,dy$.  
Zatem  
$\int_1^2 \int_1^y \frac{x}{y^2}\,dx\,dy=\int_1^2 \frac{y^2-1}{2y^2}\,dy=\frac{1}{4}$,  
$\int_2^4 \int_{y/2}^y \frac{x}{y^2}\,dx\,dy=\int_2^4 \frac{3}{8}\,dy=\frac{3}{4}$,  
$\int_4^8 \int_{y/2}^4 \frac{x}{y^2}\,dx\,dy=\int_4^8 \left(\frac{8}{y^2}-\frac{1}{8}\right)\,dy=\frac{1}{2}$.  
Wobec tego wartość całki wynosi $\frac{1}{4}+\frac{3}{4}+\frac{1}{2}=\frac{3}{2}$.

**Zadanie 5.**  
Zmienić kolejność całkowania w podanej całce, a następnie policzyć ją: $\int_0^{\sqrt{2}/2} \int_{\arcsin y}^{\arccos y} dx\,dy$.

**Odpowiedź.**  
Warunki $\arcsin y\le x\le \arccos y$ są równoważne nierównościom $y\le \sin x$ oraz $y\le \cos x$, przy czym $0\le x\le \frac{\pi}{2}$.  
Po zmianie kolejności całkowania:  
$\int_0^{\sqrt{2}/2} \int_{\arcsin y}^{\arccos y} dx\,dy=\int_0^{\pi/4} \int_0^{\sin x} dy\,dx+\int_{\pi/4}^{\pi/2} \int_0^{\cos x} dy\,dx$.  
Stąd  
$\int_0^{\pi/4} \int_0^{\sin x} dy\,dx+\int_{\pi/4}^{\pi/2} \int_0^{\cos x} dy\,dx=\int_0^{\pi/4} \sin x\,dx+\int_{\pi/4}^{\pi/2} \cos x\,dx=2-\sqrt{2}$.

## Współrzędne biegunowe

**Zadanie 6.**  
Wprowadzając współrzędne biegunowe, policzyć całkę $\iint_D \frac{dx\,dy}{(1-x^2-y^2)^2}$, gdzie $D=\{(x,y): x^2+y^2\le y,\ x\ge y\}$.

**Odpowiedź.**  
We współrzędnych biegunowych warunek $x^2+y^2\le y$ ma postać $r^2\le r\sin\varphi$, czyli $0\le r\le \sin\varphi$.  
Warunek $x\ge y$ daje $\cos\varphi\ge \sin\varphi$, więc $0\le \varphi\le \frac{\pi}{4}$.  
Zatem  
$\iint_D \frac{dx\,dy}{(1-x^2-y^2)^2}=\int_0^{\pi/4} \int_0^{\sin\varphi} \frac{r}{(1-r^2)^2}\,dr\,d\varphi$.  
Po obliczeniu całki wewnętrznej:  
$\int_0^{\sin\varphi} \frac{r}{(1-r^2)^2}\,dr=\frac{1}{2}\left(\frac{1}{1-\sin^2\varphi}-1\right)=\frac{1}{2}\left(\frac{1}{\cos^2\varphi}-1\right)=\frac{1}{2}\tan^2\varphi$.  
Stąd  
$\int_0^{\pi/4} \int_0^{\sin\varphi} \frac{r}{(1-r^2)^2}\,dr\,d\varphi=\frac{1}{2}\int_0^{\pi/4} \tan^2\varphi\,d\varphi=\frac{1}{2}\int_0^{\pi/4} \left(\frac{1}{\cos^2\varphi}-1\right)\,d\varphi=\frac{4-\pi}{8}$.

## Pole obszaru

**Zadanie 7.**  
Policzyć pole obszaru $D$ ograniczonego prostymi: $x-2y=0$, $x-2y=3$, $y=2x-9$, $y=2x-6$.

**Odpowiedź.**  
Przyjmujemy zmienne $u=x-2y$ oraz $v=2x-y$. Wtedy obszar przechodzi na prostokąt  
$0\le u\le 3$, $6\le v\le 9$.  
Jakobian przekształcenia spełnia zależność  
$\frac{\partial(u,v)}{\partial(x,y)}=1\cdot(-1)-(-2)\cdot 2=3$,  
więc $dx\,dy=\frac{1}{3}\,du\,dv$.  
Zatem  
$P(D)=\iint_D 1\,dx\,dy=\int_0^3 \int_6^9 \frac{1}{3}\,dv\,du=3$.

**Zadanie 8.**  
Policzyć pole obszaru $D$ ograniczonego krzywymi: $y=e^x$, $y=\ln x$, $x+y=1$, $x=2$.

**Odpowiedź.**  
Punkty przecięcia: $e^x=1-x$ daje $x=0$, natomiast $\ln x=1-x$ daje $x=1$.  
Pole ma więc postać  
$P(D)=\int_0^1 \bigl(e^x-(1-x)\bigr)\,dx+\int_1^2 \bigl(e^x-\ln x\bigr)\,dx$.  
Po obliczeniu:  
$\int_0^1 \bigl(e^x-(1-x)\bigr)\,dx=\left[e^x-x+\frac{x^2}{2}\right]_0^1=e-\frac{3}{2}$,  
$\int_1^2 \bigl(e^x-\ln x\bigr)\,dx=\left[e^x-x\ln x+x\right]_1^2=e^2-e+1-2\ln 2$.  
Zatem  
$P(D)=e^2-\frac{1}{2}-2\ln 2$.

**Zadanie 9.**  
Policzyć pole obszaru $D=\{(x,y): x^2+y^2\le 2x,\ y\ge x\}$.

**Odpowiedź.**  
We współrzędnych biegunowych warunek $x^2+y^2\le 2x$ przyjmuje postać $r\le 2\cos\varphi$, a warunek $y\ge x$ daje $\varphi\in\left[\frac{\pi}{4},\frac{\pi}{2}\right]$.  
Stąd  
$P(D)=\int_{\pi/4}^{\pi/2} \int_0^{2\cos\varphi} r\,dr\,d\varphi=2\int_{\pi/4}^{\pi/2} \cos^2\varphi\,d\varphi$.  
Zatem  
$P(D)=\int_{\pi/4}^{\pi/2} (1+\cos 2\varphi)\,d\varphi=\left[\varphi+\frac{\sin 2\varphi}{2}\right]_{\pi/4}^{\pi/2}=\frac{\pi}{4}-\frac{1}{2}$.

## Objętość

**Zadanie 10.**  
Korzystając z całki podwójnej obliczyć objętość słupa między powierzchnią walca o promieniu $a$, którego osią jest $Oy$, a trójkątem $OAB$, gdzie $O(0,0,0)$, $A(a,0,0)$, $B(a,a,0)$.

**Odpowiedź.**  
Walec ma równanie $x^2+z^2=a^2$, więc nad trójkątem $OAB$ wysokość słupa jest równa $z=\sqrt{a^2-x^2}$.  
Rzut na płaszczyznę $Oxy$ jest trójkątem  
$D=\{(x,y): 0\le x\le a,\ 0\le y\le x\}$.  
Zatem  
$V=\iint_D \sqrt{a^2-x^2}\,dx\,dy=\int_0^a \int_0^x \sqrt{a^2-x^2}\,dy\,dx=\int_0^a x\sqrt{a^2-x^2}\,dx$.  
Po podstawieniu $u=a^2-x^2$, $du=-2x\,dx$, otrzymujemy  
$V=\frac{1}{2}\int_0^{a^2} u^{1/2}\,du=\frac{a^3}{3}$.

**Zadanie 11.**  
Korzystając z całki podwójnej obliczyć objętość bryły ograniczonej powierzchniami: $x^2+y^2=2y$, $z=x^2+y^2$, $z=0$.

**Odpowiedź.**  
Objętość jest równa  
$V=\iint_D (x^2+y^2)\,dx\,dy$, gdzie $D=\{(x,y): x^2+y^2\le 2y\}$.  
We współrzędnych biegunowych obszar ma opis $0\le \varphi\le \pi$, $0\le r\le 2\sin\varphi$.  
Stąd  
$V=\int_0^\pi \int_0^{2\sin\varphi} r^2\cdot r\,dr\,d\varphi=\int_0^\pi \int_0^{2\sin\varphi} r^3\,dr\,d\varphi=4\int_0^\pi \sin^4\varphi\,d\varphi$.  
Ponieważ $\int_0^\pi \sin^4\varphi\,d\varphi=\frac{3\pi}{8}$, dostajemy  
$V=4\cdot \frac{3\pi}{8}=\frac{3\pi}{2}$.
