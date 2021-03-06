# Patikrinimo sąlyga if: pilna sąlyga

## Vaizdo pamoka

<iframe width="560" height="315" src="https://www.youtube.com/embed/pFPxvdYwx7c?start=6865&end=7143" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Apie pilną `if` sąlygą

Pilnoje `if` sąlygoje naudosite visas galimas `if` sąlygos dalis (`if`, `else if`, `else`).

Šiuo atveju patikrinsite kelias galimas sąlygas, bei jei niekas netiks - vistiek kažką padarysite su `else` dalimi.

## Pilnos `if` sąlygos sintaksė

```cpp
if (<pirma sąlyga>)
{
    // jeigu pirma salyga true - vykdomas čia esantis kodas
}
else if (<antra sąlyga>)
{
    // jeigu antra salyga true - vykdomas čia esantis kodas
}
else if (<trečia sąlyga>)
{
    // jeigu trečia salyga true - vykdomas čia esantis kodas
}
else {
	// jeigu sąlyga false - vykdomas čia esantis kodas
}
```

:::tip Dėl else if dalies
`else if` dalių galima dėti tiek kiek reikia. Todėl gali būti viena dalis, dvi dalys, ar daugiau, nei parodyta šiame pavyzdyje.
:::

## Pavyzdžiai

### Pavyzdys 1

Kodas:

```cpp
#include <iostream>
using namespace std;

int main()
{
	int skaicius = -3;

	if (skaicius > 0)
	{
		cout << "skaicius yra teigiamas";
	}
	else if (skaicius < 0)
	{
		cout << "skaicius yra neigiamas";
	}
	else
	{
		cout << "skaicius lygus 0";
	}

	cout << endl << "o pats skaicius: " << skaicius;
}
```

Rezultatai:

```
skaicius yra neigiamas
o pats skaicius: -3
```

### Pavyzdys 2

Kodas:

```cpp
#include <iostream>
using namespace std;

int main()
{
	int skaicius = 123;

	if (skaicius % 2 == 0)
	{
		cout << "skaicius dalinasi is 2";
	}
	else if (skaicius % 3 == 0)
	{
		cout << "skaicius dalinasi is 3";
	}
	else if (skaicius % 4 == 0)
	{
		cout << "skaicius dalinasi is 4";
	}
	else
	{
		cout << "nepavyko rasti, kad skaicius is ko nors dalintusi";
	}
}
```

Rezultatai:

```
skaicius dalinasi is 3
```

### Pavyzdys 3

Kodas:

```cpp
#include <iostream>
#include <string>
using namespace std;

int main()
{
	string vardas;
	cout << "iveskite varda: ";
	cin >> vardas;

	if (vardas == "Jonas")
	{
		cout << "Labas, Jonai";
	}
	else if (vardas == "Tomas")
	{
		cout << "labas, Tomai";
	}
	else
	{
		cout << "labas, nepazistamasis";
	}
}
```

Rezultatas 1:

```
iveskite varda: Tomas
labas, Tomai
```

Rezultatas 2:

```
iveskite varda: Petras
labas, nepazistamasis
```

Rezultatas 3:

```
iveskite varda: Giedrius
labas, nepazistamasis
```

## Užduotys

### Užduotis 1

Liepkite vartotojui įvesti skaičių. Patikrinkite:

- Ar skaičius dalinasi iš 2?
- Ar skaičius dalinasi iš 3?
- Ar skaičius dalinasi iš 4?
- Ar skaičius dalinasi iš 5?
- Ar skaičius dalinasi iš 7?
- Jeigu skaičius iš nieko nesidalina, išvesti klaidos pranešimą.

### Užduotis 2

Liepkite vartotojui įvesti du skaičius. Patikrinkite:

- Ar pirmas skaičius didesnis už antrą?
- Ar antras skaičius didesnis už pirmą?
- Jeigu nei vienas skaičius nėra didesnis už kitą - tai skaičiai yra lygūs.
