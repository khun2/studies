## Azonosságok
- kommutatív
	- A * B = B * A
- asszociatív
	- (A + B) + C = A + (B + C)
- disztributív
	- A * (B + C)  = A * B + A * C

-  A * A = A
	- {1;2} * {1;2} = {1;2}
- A + Ø = A, A * Ø = Ø
- A + H(biztos esemény) = H, A * H  = A
- A + !A = H ; A * !A = Ø
- de Morgan azonosság:
	- A * B = —A + !B

## Valószínűségszámítás (Valszám)

*Def: adott A esemény valószínűsége az a szám ami körül a relatív gyakoriság ingadozik*

### Tulajdonságok:
- O <=P(A) <= 1
- P(Ø) = 0, p(H) = 1
- A és B egymást kizáró események ha !A = B
	- 1 = P(A+!A) = P(A) + P(!A) -> P(A) = 1 P(!A) [komplementerleszámolás]
### Klasszikus valószínűségi modell
- Pl: érme: {F, Í}
	- A = 2*{min 1 db F} = {FF; FÍ; ÍF} <- 3 elem
	- eseménytér: {FF; FÍ; ÍÍ; ÍF} <- 4 elem
		- P(A) = 3/4
		- *P(A) = kedvező elemi események száma / az összes elemi esemény száma = kedvező / összes = k / n*
#### feladatok
__1.__
	A = {Páratlan prímszámot dobunk} = {3; 5}
		eseménytér: {1; 2; 3; 4; 5; 6}
		P(A) = kedvező / összes = 2/6 = 1/3
	B = {3-nál nagyobbat dobunk} = {4;5;6}
		P(B) = k/ö = 3/6 = 1/2
	C = {5-nél kisebbet} = {1;2;3;4}
		P(C) = k/ö  = 4/6 = 2/3
__2.__
	3* pénzérmadobás
	A = {min 1 F} = {FFF; FFÍ; ÍFF; FÍÍ; ÍFÍ; ÍÍF; FÍF}
		P(A) = k/ö  = 7/8