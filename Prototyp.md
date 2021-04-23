Prototyp. Marcel Wilanowicz. Data 23.04.2021.
  Zacząłem od zadelkarowania zmiennych SCREEN_HEIGHT i SCREEN_WIDTH, odpowiadających wysokości i szerokości ekranu gry(jest to niezbędne dla klasy Background, w której tło będzie generowane o stałą wartość ekranu).
W Klasie Background zainicjowałem koordynaty (0, 0), od których renderowany jest obraz tła. Klasa wczytuje background.jpg oraz jego szerokość. W funkcji update(): położenie x tła dekrementuje o stałą wartość 
prędkości tła. W momencie gdy polożenie x tła jest mniejsze od wartośi ujemnej jego szerekości(całe tło zostało przesunięte za ekran), funkcja przenosci tło na koordynaty początkowe(w ten sposób mamy złudzenie
ciągłości tła). Naszemu bohaterowi nadałem możliwość skakania: zadeklarowałem wartość prędkości skakania(z którą przemieszcza się do góry). Poprzez zmniejszanie pozycji y bohatera o tą prędkość mamy złudzenie, 
że bohater przemieszcza się do góry. Z każdym przesunięciem prędkość spada aż osiąga wartość ujemną(wtedy warunek skakania zostaje przerwany[spada] i na nowo są przypisane wartości początkowe skoku). 
Utworzyłem klasę Spike, która wczytuje obraz spike.png, jego współrzędne ramki kolizji i analogicznie jak w klasie Background, zmniejsza położenie x kolca o stałą wartość prędkości tła(kolec porusza się z tą samą prędkością co tło). 
W momencie, gdy położenie kolca jest równe ujemnej wartości jego szerokości(jest za ekranem), przypisuje mu na nowo pozycję x równą szerokości ekranu(renderuje od początku). Stworzyłem również licznik punktów z czcionką 'freesansbold.ttf' i wymiarach 20pikseli, 
jednak ten należy jeszcze dopracować(warunek zdobywania punktów). Nadałem warunek kolizji pomiędzy kolcem i bohaterem, jednak tą mechanikę również muszę dopracować(warunek kolizji i co po niej nastęouje). W produkcie końcowym dwie ostatnie rzeczy powinny być dopracowane
oraz jak postaram się stworzyć przyjazne dla użytkownika menu gry. 
