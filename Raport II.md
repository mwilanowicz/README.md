Zaczalem od zaimportowania biblioteki pygame(niezbednej do korzystania z funkcji i modulow creatora gry) i os(niezbednej do wczytywania plików/obrazów ze ścieżki).
Wstawiłem funkcje pygame.init(), która inicjuje wszystkie moduly niezbedne dla PyGame(forma zabezpieczenia oraz zaoszczędzenia czasu na ewentualnej inicjalizacji modułów).
Utworzyłem okno gry z tytułem "Geometry Crash" o rozdzielczości 600x600 pikseli.
Zadeklarowałem zmienne, które wczytują ze ścieżki tekstury wykorzytywane w grze.
Zadeklarowałem klasę "Game" wewnątrz której znajdują się informacje na temat pozycji obiektów(ewentualnej kolizji), funkcje domyślnego stanu gry, przemieszczania, skakania, zmiany stanu gry oraz funkcji "draw" za pomocą której wyświetlany jest obraz gry(wszyskie obiekty w ich aktualnym położeniu)
Zadeklarowałem funkcję główną gry, w której znajduje się pętla główna(dzięki niej gra działa, gdyż wszystkie zmiany na ekranie muszą robić się na bieżąco oraz sama gra musi wykonywać się cały czas).
Wewnątrz głównej pętli stworzyłem standardowy warunek przerwania pętli(zakończenia gry) w wyniku kliknięcią na ikonę "X" w prawym górnym rogu okna gry.
Wewnątrz głównej pętli inicjuje funkcje kolorowania ekranu gry na biało, rysowania(generowania) ekranu gry, aktualizowania stany gry przez gracza oraz jego wyświetlania na ekranie.
