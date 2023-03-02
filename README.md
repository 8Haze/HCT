--------------------------------------------------------------------------------------------------------------------------
Polish
--------------------------------------------------------------------------------------------------------------------------

dynarray - Odpowiednik std::vector, zrobiony głównie w celu przećwiczenia moich umiejętności.

deck - Odpowiednik std::deque, zaimplementowany w inny sposób, niż "standardowy". Można go określić jako bufor cykliczny o dynamicznym rozmiarze. 
Moja struktura wykazywała sporo lepszą wydajność w wykonywaniu większości operacji w porównaniu do implementacji std::deque w Visual Studio.

queue - Adaptor kolejki, wykorzystujący domyślnie hct::deck.

stack - Adaptor stosu, wykorzystujący domyślnie hct::dynarray.

sort - Głównie chodzi tu o moją własną implementację sortowania introspektywnego, które dodatkowo wykorzystuje multithreading.

scope_guard - Użyteczne narzędzie do wykonywania danych fragmentów kodu, gdy wychodzimy z jakiegoś obszaru kodu w wyniku błędu i/lub sukcesu.

rng - Pomocniczy plik, z którego można bardzo szybko uzyskać dostęp do generowania pseudolosowych liczb, gdy nie potrzebujemy ich do kryptografii ani niczego podobnego.

--------------------------------------------------------------------------------------------------------------------------
English
--------------------------------------------------------------------------------------------------------------------------

dynarray - An std::vector equivalent, made mostly with practice in mind.

deck - A data structure that was supposed to be a better std::deque. It was implemented in a circular-buffer-like way, which resulted in much better performance due to better utilization of memory caching (measured in comparison with Visual Studio's std::deque implementation). This is my proudest part of the library so far.

queue - A queue adaptor, using hct::deck by default.

stack - A stack adaptor, using hct::dynarray by default.

sort - My own implementation of an introspective sort which utilizes multithreading.

scope_guard - A very useful programming tool that helps control resources more easily.

rng - This file is mostly used for convenience to grant very quick access to random numbers when we don't need cryptography safety or anything. 
