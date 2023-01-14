dynarray - Odpowiednik std::vector, zrobiony głównie w celu przećwiczenia moich umiejętności.

deck - Odpowiednik std::deque, zaimplementowany w inny sposób, niż "standardowy". Można go określić jako bufor cykliczny o dynamicznym rozmiarze. 
Moja struktura wykazywała sporo lepszą wydajność w wykonywaniu większości operacji w porównaniu do implementacji std::deque w Visual Studio.

queue - Adaptor kolejki, wykorzystujący domyślnie hct::deck.

stack - Adaptor stosu, wykorzystujący domyślnie hct::dynarray.

sort - Głównie chodzi tu o moją własną implementację sortowania introspektywnego, które dodatkowo wykorzystuje multithreading.

scope_guard - Użyteczne narzędzie do wykonywania danych fragmentów kodu, gdy wychodzimy z jakiegoś obszaru kodu w wyniku błędu i/lub sukcesu.

rng - Pomocniczy plik, z którego można bardzo szybko uzyskać dostęp do generowania pseudolosowych liczb, gdy nie potrzebujemy ich do kryptografii ani niczego podobnego.
