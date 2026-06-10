# Zastosowania całek we współrzędnych biegunowych, walcowych i sferycznych

## Zadania

### Zadanie 1

Obliczyć pole części paraboloidy $z=x^2+y^2$ wyciętej pionowym walcem $x^2+y^2=1$.

### Zadanie 2

Dana jest górna półsfera kuli o promieniu $R$. Obliczyć pole tej części półsfery, która znajduje się wewnątrz pionowego walca o równaniu $x^2+y^2-Rx=0$.

### Zadanie 3

Obliczyć pole bocznej powierzchni stożka $z=\sqrt{x^2+y^2}$ zawartej między płaszczyznami $z=1$ i $z=2$.

### Zadanie 4

Obliczyć współrzędne środka ciężkości jednorodnej półkuli pełnej opisanej warunkami $x^2+y^2+z^2\leq R^2$, $z\geq 0$.

### Zadanie 5

Wyznaczyć środek masy jednorodnego obszaru opisanego nierównościami $x^2\leq y\leq 4$, $0\leq z\leq 4-y$.

### Zadanie 6

Obliczyć masę bryły leżącej wewnątrz walca $x^2+y^2\leq 16$, między płaszczyzną $z=0$ a stożkiem $z=2\sqrt{x^2+y^2}$, jeżeli gęstość objętościowa wynosi $\gamma(x,y,z)=x^2+y^2$.

---

## Rozwiązania

### Zadanie 1

Słowny opis obszaru: szukamy pola części paraboloidy obrotowej $z=x^2+y^2$ leżącej nad kołem jednostkowym w płaszczyźnie $xy$.

Uzasadnienie wyboru współrzędnych: wybieramy współrzędne biegunowe w rzucie na płaszczyznę $xy$, ponieważ rzut powierzchni jest kołem $x^2+y^2\leq 1$. Przyjmujemy $x=r\cos\varphi$, $y=r\sin\varphi$, gdzie $0\leq r\leq 1$, $0\leq \varphi\leq 2\pi$.

Dla powierzchni $z=f(x,y)$ mamy $dS=\sqrt{1+f_x^2+f_y^2}\,dx\,dy$. Tutaj $f(x,y)=x^2+y^2$, więc $f_x=2x$, $f_y=2y$ oraz $\sqrt{1+f_x^2+f_y^2}=\sqrt{1+4x^2+4y^2}=\sqrt{1+4r^2}$.

Całka iterowana: $S=\int_0^{2\pi}\int_0^1 \sqrt{1+4r^2}\,r\,dr\,d\varphi$.

Wynik całki wewnętrznej: $\int_0^1 r\sqrt{1+4r^2}\,dr=\frac{1}{12}(5\sqrt5-1)$.

Wynik końcowy: $S=2\pi\cdot \frac{1}{12}(5\sqrt5-1)=\boxed{\frac{\pi}{6}(5\sqrt5-1)}$.

---

### Zadanie 2

Słowny opis obszaru: szukamy pola fragmentu górnej półsfery promienia $R$, którego rzut na płaszczyznę $xy$ leży wewnątrz koła $x^2+y^2-Rx\leq 0$.

Uzasadnienie wyboru współrzędnych: wybieramy współrzędne biegunowe w rzucie na płaszczyznę $xy$, ponieważ walec ma równanie zależne od $x^2+y^2$ oraz $x$. Dla $x=r\cos\varphi$, $y=r\sin\varphi$ warunek $x^2+y^2-Rx\leq 0$ daje $r^2-Rr\cos\varphi\leq 0$, czyli $0\leq r\leq R\cos\varphi$, gdzie $-\frac{\pi}{2}\leq \varphi\leq \frac{\pi}{2}$.

Górna półsfera ma równanie $z=\sqrt{R^2-x^2-y^2}=\sqrt{R^2-r^2}$. Dla powierzchni sferycznej zapisanej jako wykres nad płaszczyzną $xy$ mamy $dS=\frac{R}{\sqrt{R^2-r^2}}\,r\,dr\,d\varphi$.

Całka iterowana: $S=\int_{-\pi/2}^{\pi/2}\int_0^{R\cos\varphi}\frac{Rr}{\sqrt{R^2-r^2}}\,dr\,d\varphi$.

Wynik całki wewnętrznej: $\int_0^{R\cos\varphi}\frac{Rr}{\sqrt{R^2-r^2}}\,dr=R^2(1-|\sin\varphi|)$.

Wynik końcowy: $S=R^2\int_{-\pi/2}^{\pi/2}(1-|\sin\varphi|)\,d\varphi=\boxed{R^2(\pi-2)}$.

---

### Zadanie 3

Słowny opis obszaru: szukamy pola bocznej powierzchni stożka $z=\sqrt{x^2+y^2}$ między poziomami $z=1$ i $z=2$.

Uzasadnienie wyboru współrzędnych: wybieramy współrzędne biegunowe w rzucie na płaszczyznę $xy$, ponieważ stożek ma postać $z=r$. Warunek $1\leq z\leq 2$ daje $1\leq r\leq 2$, a kąt pełny to $0\leq \varphi\leq 2\pi$.

Dla powierzchni $z=f(x,y)=\sqrt{x^2+y^2}$ mamy $f_x=\frac{x}{\sqrt{x^2+y^2}}$, $f_y=\frac{y}{\sqrt{x^2+y^2}}$, więc $f_x^2+f_y^2=1$. Zatem $dS=\sqrt2\,dx\,dy=\sqrt2\,r\,dr\,d\varphi$.

Całka iterowana: $S=\int_0^{2\pi}\int_1^2 \sqrt2\,r\,dr\,d\varphi$.

Wynik całki wewnętrznej: $\int_1^2 \sqrt2\,r\,dr=\frac{3\sqrt2}{2}$.

Wynik końcowy: $S=2\pi\cdot \frac{3\sqrt2}{2}=\boxed{3\pi\sqrt2}$.

---

### Zadanie 4

Słowny opis obszaru: szukamy środka ciężkości jednorodnej półkuli pełnej promienia $R$, leżącej nad płaszczyzną $xy$.

Uzasadnienie wyboru współrzędnych: wybieramy współrzędne sferyczne, ponieważ obszar jest częścią kuli. Przyjmujemy $x=\rho\sin\varphi\cos\theta$, $y=\rho\sin\varphi\sin\theta$, $z=\rho\cos\varphi$, gdzie $0\leq \rho\leq R$, $0\leq \varphi\leq \frac{\pi}{2}$, $0\leq \theta\leq 2\pi$.

Z symetrii $\bar{x}=0$ oraz $\bar{y}=0$.

Objętość: $V=\int_0^{2\pi}\int_0^{\pi/2}\int_0^R \rho^2\sin\varphi\,d\rho\,d\varphi\,d\theta$.

Wynik całki wewnętrznej objętości: $\int_0^R \rho^2\sin\varphi\,d\rho=\frac{R^3}{3}\sin\varphi$.

Wynik kolejnej całki objętości: $\int_0^{\pi/2}\frac{R^3}{3}\sin\varphi\,d\varphi=\frac{R^3}{3}$.

Wynik objętości: $V=\frac{2\pi R^3}{3}$.

Moment względem płaszczyzny $xy$: $M_{xy}=\int_0^{2\pi}\int_0^{\pi/2}\int_0^R \rho\cos\varphi\cdot \rho^2\sin\varphi\,d\rho\,d\varphi\,d\theta$.

Wynik całki wewnętrznej momentu: $\int_0^R \rho^3\cos\varphi\sin\varphi\,d\rho=\frac{R^4}{4}\cos\varphi\sin\varphi$.

Wynik kolejnej całki momentu: $\int_0^{\pi/2}\frac{R^4}{4}\cos\varphi\sin\varphi\,d\varphi=\frac{R^4}{8}$.

Wynik momentu: $M_{xy}=2\pi\cdot \frac{R^4}{8}=\frac{\pi R^4}{4}$.

Współrzędna $\bar{z}$: $\bar{z}=\frac{M_{xy}}{V}=\frac{\pi R^4/4}{2\pi R^3/3}=\frac{3R}{8}$.

Wynik końcowy: $\boxed{S=\left(0,0,\frac{3R}{8}\right)}$.

---

### Zadanie 5

Słowny opis obszaru: szukamy środka masy jednorodnej bryły, której rzut na płaszczyznę $xy$ jest obszarem między parabolą $y=x^2$ a prostą $y=4$, a wysokość jest ograniczona przez $0\leq z\leq 4-y$.

Uzasadnienie wyboru współrzędnych: wybieramy współrzędne kartezjańskie bez przekształceń, ponieważ podstawa jest naturalnie opisana nierównościami $x^2\leq y\leq 4$, a górna granica jest prostą funkcją $y$.

Opis obszaru: $-2\leq x\leq 2$, $x^2\leq y\leq 4$, $0\leq z\leq 4-y$.

Objętość: $V=\int_{-2}^{2}\int_{x^2}^{4}\int_0^{4-y}1\,dz\,dy\,dx$.

Wynik całki wewnętrznej objętości: $\int_0^{4-y}1\,dz=4-y$.

Wynik kolejnej całki objętości: $\int_{x^2}^{4}(4-y)\,dy=8-4x^2+\frac{x^4}{2}$.

Wynik objętości: $V=\frac{256}{15}$.

Moment względem płaszczyzny $yz$: z symetrii względem osi $y$ mamy $M_{yz}=0$, więc $\bar{x}=0$.

Moment względem płaszczyzny $xz$: $M_{xz}=\int_{-2}^{2}\int_{x^2}^{4}\int_0^{4-y}y\,dz\,dy\,dx$.

Wynik całki wewnętrznej: $\int_0^{4-y}y\,dz=y(4-y)$.

Wynik kolejnej całki: $\int_{x^2}^{4}y(4-y)\,dy=\frac{32}{3}-2x^4+\frac{x^6}{3}$.

Wynik momentu: $M_{xz}=\frac{1024}{35}$.

Moment względem płaszczyzny $xy$: $M_{xy}=\int_{-2}^{2}\int_{x^2}^{4}\int_0^{4-y}z\,dz\,dy\,dx$.

Wynik całki wewnętrznej: $\int_0^{4-y}z\,dz=\frac{(4-y)^2}{2}$.

Wynik kolejnej całki: $\int_{x^2}^{4}\frac{(4-y)^2}{2}\,dy=-\frac{x^6}{6}+2x^4-8x^2+\frac{32}{3}$.

Wynik momentu: $M_{xy}=\frac{2048}{105}$.

Współrzędne środka masy: $\bar{x}=0$, $\bar{y}=\frac{M_{xz}}{V}=\frac{12}{7}$, $\bar{z}=\frac{M_{xy}}{V}=\frac{8}{7}$.

Wynik końcowy: $\boxed{S=\left(0,\frac{12}{7},\frac{8}{7}\right)}$.

---

### Zadanie 6

Słowny opis obszaru: szukamy masy bryły leżącej wewnątrz walca promienia $4$, nad płaszczyzną $z=0$ i pod stożkiem $z=2\sqrt{x^2+y^2}$, przy gęstości $\gamma(x,y,z)=x^2+y^2$.

Uzasadnienie wyboru współrzędnych: wybieramy współrzędne walcowe, ponieważ zarówno walec, stożek, jak i gęstość zależą od $r=\sqrt{x^2+y^2}$. Mamy $x^2+y^2=r^2$, $dx\,dy\,dz=r\,dz\,dr\,d\varphi$.

Opis obszaru: $0\leq \varphi\leq 2\pi$, $0\leq r\leq 4$, $0\leq z\leq 2r$.

Całka iterowana: $M=\int_0^{2\pi}\int_0^4\int_0^{2r} r^2\cdot r\,dz\,dr\,d\varphi=\int_0^{2\pi}\int_0^4\int_0^{2r}r^3\,dz\,dr\,d\varphi$.

Wynik całki wewnętrznej: $\int_0^{2r}r^3\,dz=2r^4$.

Wynik kolejnej całki: $\int_0^4 2r^4\,dr=\frac{2048}{5}$.

Wynik końcowy: $M=2\pi\cdot \frac{2048}{5}=\boxed{\frac{4096\pi}{5}}$.

---

## Odpowiedzi

Zadanie 1. $\boxed{S=\frac{\pi}{6}(5\sqrt5-1)}$.

Zadanie 2. $\boxed{S=R^2(\pi-2)}$.

Zadanie 3. $\boxed{S=3\pi\sqrt2}$.

Zadanie 4. $\boxed{S=\left(0,0,\frac{3R}{8}\right)}$.

Zadanie 5. $\boxed{S=\left(0,\frac{12}{7},\frac{8}{7}\right)}$.

Zadanie 6. $\boxed{M=\frac{4096\pi}{5}}$.