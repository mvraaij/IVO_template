# Achtergrond: Riemannsommen
In dit hoofdstuk staat de achtergrond van integralen: Riemannsommen en hoe deze leiden tot een integraal.

We hebben gezien dat de integraal van een functie $f$ tussen $x=a$ en $x=b$ gelijk is aan $\int_a^b f(x)dx$.
Hierbij wordt eigenlijk een som genomen van oneindig veel rechthoekjes van dikte $dx$ en hoogte $f(x)$ voor waarden tussen $x=a$ en $x=b$.
Dit proces kunnen we laten zien als een limietproces.
De limiet kennen we al van de afgeleide:
$$ f'(x) = \lim_{h\to 0} \frac{f(x+h)-f(x)}{h}$$
Hetzelfde kunnen we doen met de integraal.

We beginnen met het verdelen van het interval $[a,b]$ in een aantal blokjes.
We nemen nu $n+1$ punten $x_0$ tot en met $x_n$ met $a = x_0 < x_1 < x_2 < ... < x_{n-1} < x_n = b$.
Voor het gemak nemen we de punten $x_i$ allemaal met gelijke afstand: $x_i =x_0 + i \cdot \Delta x$ voor elke $i$ tussen $0$ en $n$, waarbij $\Delta x$ de stapgroote is.
Maar wat is nu de stapgrootte die we nodig hebben?
We willen dat $x_n = b$ en $x_0 = a$.
Wanneer we dit invullen krijgen we 
$$\begin{align*} b &= x_0 + n \cdot \Delta x \\
b &= a + n \cdot \Delta x \\
n \cdot \Delta x &= b-a \\
\Delta x &= \frac{b-a}{n}
\end{align*}$$
We hebben nu een breedte $\Delta x$ van ons rechthoekje, maar we moeten ook nog een hoogte bepalen.
Tussen twee punten $x_i$ en $x_{i+1}$ kan een functie meerdere waarden aannemen.
Laten we twee opties bekijken: de onderkant en de bovenkant van het interval.
We hebben $$L = \sum_{i=0}^{n-1} f(x_i) \Delta x  $$ en $$R = \sum_{i=0}^{n-1} f(x_{i+1}) \Delta x$$

Deze $L$ noemen we de linkersom en de $R$ noemen we de rechtersom. 

_Deze theorie is vrij hooggegrepen, daar ben ik mij van bewust.
Dit is nog een voorlopige versie._