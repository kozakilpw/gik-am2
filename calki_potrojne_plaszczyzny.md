# Całki potrójne — obszary zadane przez wierzchołki i płaszczyzny

## Zadania

### $\iiint$ 1

Obszar $E_1$ jest prostopadłościanem o wierzchołkach $(0,0,0)$, $(3,0,0)$, $(0,2,0)$, $(3,2,0)$, $(0,0,4)$, $(3,0,4)$, $(0,2,4)$, $(3,2,4)$. Obliczyć objętość obszaru $E_1$.

### $\iiint$ 2

Obszar $E_2$ jest ostrosłupem o wierzchołkach $(0,0,0)$, $(4,0,0)$, $(0,3,0)$, $(0,0,6)$. Gęstość dana jest wzorem $\rho(x,y,z)=x+y+z$. Obliczyć masę bryły.

### $\iiint$ 3

Obszar $E_3$ jest jednorodnym ostrosłupem o wierzchołkach $(0,0,0)$, $(2,0,0)$, $(0,5,0)$, $(0,0,4)$. Obliczyć środek ciężkości bryły.

### $\iiint$ 4

Obszar $E_4$ powstaje z prostopadłościanu bazowego $0\leq x\leq 2$, $0\leq y\leq 3$, $z\geq 0$, ściętego od góry płaszczyzną przechodzącą przez punkty $(6,0,0)$, $(0,6,0)$, $(0,0,6)$. Gęstość dana jest wzorem $\rho(x,y,z)=2+z$. Obliczyć masę bryły.

### $\iiint$ 5

Obszar $E_5$ powstaje z prostopadłościanu bazowego $0\leq x\leq 4$, $0\leq y\leq 2$, $z\geq 0$, ściętego od góry płaszczyzną przechodzącą przez punkty $(10,0,0)$, $(0,10,0)$, $(0,0,5)$. Gęstość jest stała: $\rho=1$. Obliczyć środek ciężkości bryły.

---

## Rozwiązania

### $\iiint$ 1

Słowny opis obszaru: prostopadłościan ograniczony płaszczyznami $x=0$, $x=3$, $y=0$, $y=2$, $z=0$, $z=4$.

Uzasadnienie wyboru współrzędnych: wybieramy współrzędne kartezjańskie bez przekształceń, ponieważ wszystkie ograniczenia są równoległe do osi układu.

Wyznaczenie górnej płaszczyzny: bierzemy punkty $P=(0,0,4)$, $Q=(3,0,4)$, $R=(0,2,4)$. Dla dowolnego punktu $X=(x,y,z)$ leżącego w tej samej płaszczyźnie wektory $\overrightarrow{PX}$, $\overrightarrow{PQ}$, $\overrightarrow{PR}$ są liniowo zależne. Dlatego wyznacznik z ich współrzędnych musi być równy $0$. Odejmowania we współrzędnych wynikają z tworzenia wektorów: $\overrightarrow{PX}=X-P$, $\overrightarrow{PQ}=Q-P$, $\overrightarrow{PR}=R-P$.

$$
\begin{vmatrix}
x-0 & y-0 & z-4\\
3-0 & 0-0 & 4-4\\
0-0 & 2-0 & 4-4
\end{vmatrix}=0.
$$

Czyli $\begin{vmatrix}x&y&z-4\\3&0&0\\0&2&0\end{vmatrix}=0$, więc $6(z-4)=0$, a zatem $z=4$.

Opis obszaru: $0\leq x\leq 3$, $0\leq y\leq 2$, $0\leq z\leq 4$.

Całka iterowana: $V=\int_0^3\int_0^2\int_0^4 1\,dz\,dy\,dx$.

Wynik całki wewnętrznej: $\int_0^4 1\,dz=4$.

Wynik kolejnej całki: $\int_0^2 4\,dy=8$.

Wynik końcowy: $\boxed{V=24}$.

---

### $\iiint$ 2

Słowny opis obszaru: ostrosłup ograniczony płaszczyznami współrzędnych oraz płaszczyzną przechodzącą przez punkty $(4,0,0)$, $(0,3,0)$, $(0,0,6)$.

Uzasadnienie wyboru współrzędnych: wybieramy współrzędne kartezjańskie bez przekształceń, ponieważ bryła jest ograniczona płaszczyznami współrzędnych i jedną płaszczyzną ukośną.

Wyznaczenie płaszczyzny: bierzemy punkty $P=(4,0,0)$, $Q=(0,3,0)$, $R=(0,0,6)$. Dla dowolnego punktu $X=(x,y,z)$ leżącego w tej samej płaszczyźnie wektory $\overrightarrow{PX}=X-P$, $\overrightarrow{PQ}=Q-P$, $\overrightarrow{PR}=R-P$ są liniowo zależne. Stąd:

$$
\begin{vmatrix}
x-4 & y-0 & z-0\\
0-4 & 3-0 & 0-0\\
0-4 & 0-0 & 6-0
\end{vmatrix}=0.
$$

Czyli $\begin{vmatrix}x-4&y&z\\-4&3&0\\-4&0&6\end{vmatrix}=0$.

Po rozwinięciu: $18x+24y+12z-72=0$. Dzielimy przez $72$ i dostajemy $\frac{x}{4}+\frac{y}{3}+\frac{z}{6}=1$, czyli $z=6-\frac32x-2y$.

Opis obszaru: $0\leq x\leq 4$, $0\leq y\leq 3-\frac34x$, $0\leq z\leq 6-\frac32x-2y$.

Całka iterowana: $M=\int_0^4\int_0^{3-\frac34x}\int_0^{6-\frac32x-2y}(x+y+z)\,dz\,dy\,dx$.

Wynik całki wewnętrznej: dla $h=6-\frac32x-2y$ mamy $\int_0^h(x+y+z)\,dz=(x+y)h+\frac{h^2}{2}$.

Wynik kolejnej całki: $\int_0^{3-\frac34x}\left((x+y)h+\frac{h^2}{2}\right)dy=\frac{9x^3}{64}+\frac{9x^2}{16}-\frac{45x}{4}+27$.

Wynik końcowy: $\boxed{M=39}$.

---

### $\iiint$ 3

Słowny opis obszaru: jednorodny ostrosłup ograniczony płaszczyznami współrzędnych oraz płaszczyzną przechodzącą przez punkty $(2,0,0)$, $(0,5,0)$, $(0,0,4)$.

Uzasadnienie wyboru współrzędnych: wybieramy współrzędne kartezjańskie bez przekształceń, ponieważ bryła jest ograniczona płaszczyznami współrzędnych i jedną płaszczyzną ukośną.

Wyznaczenie płaszczyzny: bierzemy punkty $P=(2,0,0)$, $Q=(0,5,0)$, $R=(0,0,4)$. Dla dowolnego punktu $X=(x,y,z)$ leżącego w tej samej płaszczyźnie wektory $\overrightarrow{PX}=X-P$, $\overrightarrow{PQ}=Q-P$, $\overrightarrow{PR}=R-P$ są liniowo zależne. Stąd:

$$
\begin{vmatrix}
x-2 & y-0 & z-0\\
0-2 & 5-0 & 0-0\\
0-2 & 0-0 & 4-0
\end{vmatrix}=0.
$$

Czyli $\begin{vmatrix}x-2&y&z\\-2&5&0\\-2&0&4\end{vmatrix}=0$.

Po rozwinięciu: $20x+8y+10z-40=0$. Dzielimy przez $40$ i dostajemy $\frac{x}{2}+\frac{y}{5}+\frac{z}{4}=1$, czyli $z=4-2x-\frac45y$.

Opis obszaru: $0\leq x\leq 2$, $0\leq y\leq 5-\frac52x$, $0\leq z\leq 4-2x-\frac45y$.

Objętość: $V=\int_0^2\int_0^{5-\frac52x}\int_0^{4-2x-\frac45y}1\,dz\,dy\,dx$.

Wynik całki wewnętrznej: $\int_0^{4-2x-\frac45y}1\,dz=4-2x-\frac45y$.

Wynik kolejnej całki: $\int_0^{5-\frac52x}\left(4-2x-\frac45y\right)dy=\frac52(2-x)^2$.

Wynik objętości: $V=\frac{20}{3}$.

Moment względem płaszczyzny $yz$: $M_{yz}=\int_0^2\int_0^{5-\frac52x}\int_0^{4-2x-\frac45y}x\,dz\,dy\,dx$.

Wynik całki wewnętrznej: $\int_0^{4-2x-\frac45y}x\,dz=x\left(4-2x-\frac45y\right)$.

Wynik kolejnej całki: $\int_0^{5-\frac52x}x\left(4-2x-\frac45y\right)dy=\frac52x(2-x)^2$.

Wynik momentu: $M_{yz}=\frac{10}{3}$.

Moment względem płaszczyzny $xz$: $M_{xz}=\int_0^2\int_0^{5-\frac52x}\int_0^{4-2x-\frac45y}y\,dz\,dy\,dx$.

Wynik całki wewnętrznej: $\int_0^{4-2x-\frac45y}y\,dz=y\left(4-2x-\frac45y\right)$.

Wynik kolejnej całki: $\int_0^{5-\frac52x}y\left(4-2x-\frac45y\right)dy=\frac{25}{12}(2-x)^3$.

Wynik momentu: $M_{xz}=\frac{25}{3}$.

Moment względem płaszczyzny $xy$: $M_{xy}=\int_0^2\int_0^{5-\frac52x}\int_0^{4-2x-\frac45y}z\,dz\,dy\,dx$.

Wynik całki wewnętrznej: $\int_0^{4-2x-\frac45y}z\,dz=\frac12\left(4-2x-\frac45y\right)^2$.

Wynik kolejnej całki: $\int_0^{5-\frac52x}\frac12\left(4-2x-\frac45y\right)^2dy=\frac53(2-x)^3$.

Wynik momentu: $M_{xy}=\frac{20}{3}$.

Wynik końcowy: $\bar{x}=\frac{M_{yz}}{V}=\frac12$, $\bar{y}=\frac{M_{xz}}{V}=\frac54$, $\bar{z}=\frac{M_{xy}}{V}=1$, więc $\boxed{S=\left(\frac12,\frac54,1\right)}$.

---

### $\iiint$ 4

Słowny opis obszaru: prostopadłościan bazowy $0\leq x\leq 2$, $0\leq y\leq 3$, $z\geq 0$, ścięty od góry płaszczyzną ukośną przechodzącą przez punkty $(6,0,0)$, $(0,6,0)$, $(0,0,6)$.

Uzasadnienie wyboru współrzędnych: wybieramy współrzędne kartezjańskie bez przekształceń, ponieważ rzut na płaszczyznę $xy$ jest prostokątem, a górne ograniczenie jest płaszczyzną.

Wyznaczenie płaszczyzny: bierzemy punkty $P=(6,0,0)$, $Q=(0,6,0)$, $R=(0,0,6)$. Dla dowolnego punktu $X=(x,y,z)$ leżącego w tej samej płaszczyźnie wektory $\overrightarrow{PX}=X-P$, $\overrightarrow{PQ}=Q-P$, $\overrightarrow{PR}=R-P$ są liniowo zależne. Stąd:

$$
\begin{vmatrix}
x-6 & y-0 & z-0\\
0-6 & 6-0 & 0-0\\
0-6 & 0-0 & 6-0
\end{vmatrix}=0.
$$

Czyli $\begin{vmatrix}x-6&y&z\\-6&6&0\\-6&0&6\end{vmatrix}=0$.

Po rozwinięciu: $36x+36y+36z-216=0$. Dzielimy przez $36$ i dostajemy $x+y+z=6$, czyli $z=6-x-y$.

Opis obszaru: $0\leq x\leq 2$, $0\leq y\leq 3$, $0\leq z\leq 6-x-y$.

Całka iterowana: $M=\int_0^2\int_0^3\int_0^{6-x-y}(2+z)\,dz\,dy\,dx$.

Wynik całki wewnętrznej: $\int_0^{6-x-y}(2+z)\,dz=2(6-x-y)+\frac{(6-x-y)^2}{2}$.

Wynik kolejnej całki: $\int_0^3\left(2(6-x-y)+\frac{(6-x-y)^2}{2}\right)dy=\frac32x^2-\frac{39}{2}x+\frac{117}{2}$.

Wynik końcowy: $\boxed{M=82}$.

---

### $\iiint$ 5

Słowny opis obszaru: prostopadłościan bazowy $0\leq x\leq 4$, $0\leq y\leq 2$, $z\geq 0$, ścięty od góry płaszczyzną ukośną przechodzącą przez punkty $(10,0,0)$, $(0,10,0)$, $(0,0,5)$.

Uzasadnienie wyboru współrzędnych: wybieramy współrzędne kartezjańskie bez przekształceń, ponieważ rzut na płaszczyznę $xy$ jest prostokątem, a górne ograniczenie jest płaszczyzną.

Wyznaczenie płaszczyzny: bierzemy punkty $P=(10,0,0)$, $Q=(0,10,0)$, $R=(0,0,5)$. Dla dowolnego punktu $X=(x,y,z)$ leżącego w tej samej płaszczyźnie wektory $\overrightarrow{PX}=X-P$, $\overrightarrow{PQ}=Q-P$, $\overrightarrow{PR}=R-P$ są liniowo zależne. Stąd:

$$
\begin{vmatrix}
x-10 & y-0 & z-0\\
0-10 & 10-0 & 0-0\\
0-10 & 0-0 & 5-0
\end{vmatrix}=0.
$$

Czyli $\begin{vmatrix}x-10&y&z\\-10&10&0\\-10&0&5\end{vmatrix}=0$.

Po rozwinięciu: $50x+50y+100z-500=0$. Dzielimy przez $50$ i dostajemy $x+y+2z=10$, czyli $z=5-\frac{x}{2}-\frac{y}{2}$.

Opis obszaru: $0\leq x\leq 4$, $0\leq y\leq 2$, $0\leq z\leq 5-\frac{x}{2}-\frac{y}{2}$.

Objętość: $V=\int_0^4\int_0^2\int_0^{5-\frac{x}{2}-\frac{y}{2}}1\,dz\,dy\,dx$.

Wynik całki wewnętrznej: $\int_0^{5-\frac{x}{2}-\frac{y}{2}}1\,dz=5-\frac{x}{2}-\frac{y}{2}$.

Wynik kolejnej całki: $\int_0^2\left(5-\frac{x}{2}-\frac{y}{2}\right)dy=9-x$.

Wynik objętości: $V=28$.

Moment względem płaszczyzny $yz$: $M_{yz}=\int_0^4\int_0^2\int_0^{5-\frac{x}{2}-\frac{y}{2}}x\,dz\,dy\,dx$.

Wynik całki wewnętrznej: $\int_0^{5-\frac{x}{2}-\frac{y}{2}}x\,dz=x\left(5-\frac{x}{2}-\frac{y}{2}\right)$.

Wynik kolejnej całki: $\int_0^2x\left(5-\frac{x}{2}-\frac{y}{2}\right)dy=-x^2+9x$.

Wynik momentu: $M_{yz}=\frac{152}{3}$.

Moment względem płaszczyzny $xz$: $M_{xz}=\int_0^4\int_0^2\int_0^{5-\frac{x}{2}-\frac{y}{2}}y\,dz\,dy\,dx$.

Wynik całki wewnętrznej: $\int_0^{5-\frac{x}{2}-\frac{y}{2}}y\,dz=y\left(5-\frac{x}{2}-\frac{y}{2}\right)$.

Wynik kolejnej całki: $\int_0^2y\left(5-\frac{x}{2}-\frac{y}{2}\right)dy=\frac{26}{3}-x$.

Wynik momentu: $M_{xz}=\frac{80}{3}$.

Moment względem płaszczyzny $xy$: $M_{xy}=\int_0^4\int_0^2\int_0^{5-\frac{x}{2}-\frac{y}{2}}z\,dz\,dy\,dx$.

Wynik całki wewnętrznej: $\int_0^{5-\frac{x}{2}-\frac{y}{2}}z\,dz=\frac12\left(5-\frac{x}{2}-\frac{y}{2}\right)^2$.

Wynik kolejnej całki: $\int_0^2\frac12\left(5-\frac{x}{2}-\frac{y}{2}\right)^2dy=\frac{x^2}{4}-\frac92x+\frac{61}{3}$.

Wynik momentu: $M_{xy}=\frac{152}{3}$.

Wynik końcowy: $\bar{x}=\frac{M_{yz}}{V}=\frac{38}{21}$, $\bar{y}=\frac{M_{xz}}{V}=\frac{20}{21}$, $\bar{z}=\frac{M_{xy}}{V}=\frac{38}{21}$, więc $\boxed{S=\left(\frac{38}{21},\frac{20}{21},\frac{38}{21}\right)}$.

---

## Odpowiedzi

$\iiint$ 1. $\boxed{V=24}$.

$\iiint$ 2. $\boxed{M=39}$.

$\iiint$ 3. $\boxed{S=\left(\frac12,\frac54,1\right)}$.

$\iiint$ 4. $\boxed{M=82}$.

$\iiint$ 5. $\boxed{S=\left(\frac{38}{21},\frac{20}{21},\frac{38}{21}\right)}$.