# Wat is een integraal?
Dit hoofdstuk gaat over het concept integraal: wat is het, hoe gebruiken we het?

We pakken een voorbeeld uit de natuurkunde: verplaatsing en snelheid.
Waarschijnlijk weet je nog de formule "$v=\frac{s}{t}$" waarmee je de (gemiddelde) snelheid kan berekenen wanneer je de afstand en tijd weet tussen het begin- en eindpunt.

Deze formule werkt alleen als de snelheid constant is, of je de gemiddelde snelheid wilt berekenen.
Als dit niet het geval is, maar je een formule $s(t)$ voor de afstand hebt, dan geldt dat de snelheid $v(t)=s'(t)$. Oftewel: de snelheid is de afgeleide van de afstand.

Het kan ook voorkomen dat je het omgekeerde probleem hebt: je hebt de snelheid als functie van de tijd, maar je wilt de afstand weten.
In de auto heb je bijvoorbeeld een snelheidsmeter zitten.
Deze snelheid kan je dan aflezen en in een grafiek zetten.
Wil je nu de afstand bepalen die de auto heeft afgelegd tussen twee tijdstippen kan dit op meerdere manieren:
1. Maak verschillende raaklijnen aan de grafiek, en bereken zo de gemiddelde snelheid om de afstand te berekenen met $s = v_{gem}\cdot t$. 
2. Weet je de oppervlakte onder de $v,t$ grafiek, dan is de afstand $s$ gelijk aan deze oppervlakte.  

Bij een constante of lineaire snelheid is optie 2 krijg je de oppervlakte van een rechthoek of driehoek.
Helaas is in de werkelijkheid de snelheid niet vaak constant of lineair, maar volgt deze een ander verloop.
In dat geval wordt de oppervlakte bepalen wat lastiger.

Dit is precies waar integralen nuttig zijn: de integraal van een functie geeft je de oppervlakte tussen de grafiek en de $x$-as tussen twee punten.
Een integraal wordt aangegeven met het symbool $\int$ en gebruik je als volgt.
Stel je hebt een functie $f$ en $V$ het vlak onder de grafiek van $f$ tussen $x=a$ en $x=b$. 
Dan is de oppervlakte $O(V)$ gelijk aan de _____integraal over $f(x)$ tussen $a$ en $b$_____:  
$$\int_a^b  f(x)dx$$
In deze formulering zie je al het begin- en eindpunt $x=a$ en $x=b$ bij het integraal teken staan. 
De functie $f(x)$ lijkt vermenigvuldigd te worden met een of andere '$dx$'.
De integraal neemt namelijk eigenlijk een oneindig dun strookje aan van dikte $dx$ en hoogte $f(x)$ en telt al deze strookjes bij elkaar op.

In het begin van het voorbeeld hadden we opgeschreven dat $v(t)=s'(t)$. 
We wilden weten wat $s(t)$ was in termen van $v(t)$.
We hebben dus een functie $s(t)$ nodig zodat $s'(t) = v(t)$.
Oftewel, we wilden een inversie operatie krijgen van de afgeleide. 
Tegelijkertijd bleek de afstand hetzelfde te zijn aan de oppervlakte onder de grafiek van $v(t)$ en dus die integraal.
De integraal is dus eigenlijk de inverse van een afgeleide!

## Hoe bereken je nou deze integraal?
Als we de integraal willen uitrekenen, moeten we een soort omgekeerde afgeleide kunnen bepalen. 
Hiervoor berekenen we de **primitieve** van een functie.
Een functie $f(x)$ heeft primitieve $F(x)$ als geldt dat $F'(x) = f(x)$.
Dit is precies het probleem van het voorbeeld.

Dit kunnen we doen door de lijst van standaardafgeleiden om te draaien.

Voorbeeld:\
De afgeleide van $f(x) = x^n$ is gelijk aan $f'(x) = n x^{n-1}$.\
De primitieve van $g(x) = x^{n}$ is dus $G(x) = \frac{1}{n+1} x^{n+1}$. \
Check: afgeleide $G'(x)= \frac{n+1}{n+1} x^{n+1-1} = 1 \cdot x^n = x^n = g(x)$.

Hoe combineren we nu de primitieve en de integraal?
De integraal $\int_a^b f(x)dx$ is gelijk aan $$ \int_a^b f(x)dx = F(b)-F(a)$$ met $F(x)$ de primitieve van $f(x)$.


