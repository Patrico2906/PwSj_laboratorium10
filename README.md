# Programowanie w językach skryptowych, Python
Laboratorium 8
UWAGA: Utwórz plik `mojeklasy.py`. Wpisz w pliku następujące instrukcje:
def testy():
 pass
if __name__ == "__main__":
 testy()
W funkcji testy() będzie znajdował się program testowy, w którym będą deklaracje obiektów oraz
czynności wykonywane na obiektach. W Python nie potrzebna jest funkcja startowa, ale dobra
praktyka wskazuje, aby takiej funkcji używać (u nas to jest właśnie testy())
Zadanie 1. Zdefiniuj klasę Student(), która zawiera pola (niestatyczne): imię, nazwisko, nr_indeksu,
kierunek. Klasa ma posiadać __init__(), w którym podczas tworzenia instancji (obiektu) przypisywane
będą wartości do wskazanych pól. Pole nr_indeksu powinno być prywatne. Pokaż na obiekcie, że nie
można się do tego pola odwołać. Posługując się przeciążoną metodą __str__() napisz procedurę
drukująca pola obiektu (w kodzie procedury bez print()) przy podaniu obiektu do print().
Zadanie 2. Dla klasy Student() z zad.1 napisz przeciążoną metodę porównującą dwa obiekty:
mniejszy->większy oraz równy->równy. Procedury mają porównywać pola zawierające imiona i
nazwiska, np. jeżeli stduent1 ma nazwisko Adamczyk a student2 ma nazwisko Bakuła metoda ma
zwracać True (bo student1 < student2).
Zadanie 3. Dodaj do klasy Student() prywatne pole statyczne o nazwie licznik. Napisz metodę
getLicznik(), która będzie zwracała wartość licznika. Pokaż, że licznik funkcjonuje przy wywołaniu dla
3 obiektów.
Zadanie 4. Zdefiniuj klasę StudentInformatyki(), która dziedziczy po klasie Student(). Student
informatyki jawnie wykorzystuje konstruktor klasy Student() (super()). Dodatkowo ma pole
specjalność a pole kierunek wypełnione jest wstępnie wartością „IIS”.
Zadanie 5. Napisz funkcję – dekorator o nazwie rok_drugi, która będzie dodatkową metodą klasy
Student(). Dekorator będzie miał parametr: self. Dekorator ma drukować właściwości obiektu klasy
Student() (Patrz zadanie 1 i __str__()) w taki sposób, że będzie dodawał wymienioną informację o
roku studiów. Zauważ, że dekorator może być wykorzystany tylko dla „drukowania” studenta II-giego
roku. Jak to zmienić?
