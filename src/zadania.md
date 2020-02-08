
## Zadania tablice - rozgrzewka

### Jednowymiarowe

#### Zadanie 1

Mając do dyspozycji tablicę ze zwierzętami, wypisz kolejne zwierzę w konsoli.

```javascript 
const animals = ["cat", "shrimp", "giraffe"];
```

#### Zadanie 2

Napisz funkcję addArrays, która ma przyjmować dwa argumenty - dwie tablice zawierające liczby całkowite. Funkcja ta ma zwracać również tablicę, która będzie wynikiem dodawania każdego elementu o tym samym indeksie. Jeżeli, tablice nie są równe, elementy nadmiarowe są przepisywane do nowej tablicy.


```javascript 
addArrays([4,0,1,3,4], [1,9,6,7,8,17]) => [5,9,7,10,12,17]
addArrays([8,3,22], [1,3,2]) => [9,6,24]
addArrays([2,3,1,5,3,5], [3,1,76,1]) => [5,4,77,6,3,5]
```

### Dwuwymiarowe

#### Zadanie 3

Napisz funkcje print2DArray, która będzie przyjmować jako argument tablicę dwuwymiarową. Następnie funkcja ma wypisać w konsoli zawartość tej tablicy.


```javascript 
print2dArray([[4,0],[1,3,4]]) //4, 0, 1, 3, 4
```

## Rest i spread - przypomnienie

## `...a` Operator rozsypania i reszty ( spread and rest )

### Rozsypanie napisu

> kolejność

#### Przypisz do stałej napis `Hello FED` i rozsyp go w `console.log`

```javascript

```

### Rozsypanie tablicy

#### Stwórz tablicę `users` skłądającą się z tablic `admins` i `writers` oraz dodatkowego elementu o wartości `Helm`

```javascript
   const admins = ['Sebastian', 'Robert'];
   const writers = ['Stanislav', 'Vladimir'];
```

### Rozsypanie tablicy do argumentów funkcji

#### Przekształć funkcję w strzałkową i użyj rozsypanej tablicy jako argument podczas wywołania

```javascript
const numbers = [20, 22];

function add(a, b) {
  let floatB = parseFloat(a);
  let floatA = parseFloat(b);
  return a + b
}
//wywołanie w console log
```

### Operator reszty

#### Stwórz funkcję strzałkową `logAmount` która policzy wszystkie argumenty przekazane podczas wywołania i wyświetli je w konsoli

```javascript
  logAmount(1,5,7,9,5); //5
  logAmount(1,7,9,5); //4
```

## Obiekty - temat główny

## Obiekt `{ }`

### Skrótowy zapis klucza i wartości

#### Stwórz obiekt z kluczami `name` i `surname` używając podanych wartości

```javascript
const name = "Bruce";
const surname = "Willis";
```

### Napis jako klucz w obiekcie

#### Stwórz obiekt z kluczem jako wartością z `superKey` oraz wartością z `superValue`

```javascript
const superKey = "name";
const superValue = "Bruce";
```

### Metody

#### Stwórz obiekt z kluczami `name` i `surname` używając podanych wartości oraz metodą `printFullName` następnie wywołaj tą metodę

```javascript
const name = "Bruce";
const surname = "Willis";
```

### Metoda `get`


> Nie może pojawiać się w itarale objektu z innym getem lub właściwością o takich samych nazwach ({ get x() { }, get x() { } } oraz { x: ..., get x() { } } są niedozwolone).

#### Dopisz metodę pobierającą `name`

```javascript
  const user = {
  name : 'Bruce';
    ...
  }
```

### Metoda `set`

#### Dopisz metodę ustawiającą `name`

```javascript
  const user = {
  name : 'Bruce';
    ...
  }
```

## Klasy

### Definicja klasy i jej typ

#### Stwórz klasę o nazwie `User` następnie i wywołaj kod poniżej. Jak sądzisz jaki będzie typ?

```javascript
  console.log( typeof User );
```

### Konstruktor

#### Dodaj konstruktor z dwoma parametrami `name` oraz `surname` następnie stórz obiek z definicji klasy używając `new`

```javascript
  console.log( obiektUser )
```

### Metody

#### Dodaj metodę `printName` wypisującą imię w konsoli następnie ją przetestuj

```javascript
//FED
```

### Dziedziczenie

#### Stwórz klasę `Admin` która dziedziczy po klasie `User` oraz rozszerza jej konstruktor o  atrybut `access_level`.

```javascript
 const Jacek = new Admin('name','surname','access_5');
```

### Rozszerzanie funkcjonalności klasy poprzez dziedziczenie

#### W klasie `admin` dopisz metodę `printAccesLevel`

```javascript
 const Jacek = new Admin('name','surname','access_5');
```

### Nadpisywanie funkcjonalności klasy poprzez dziedziczenie

#### W klasie `admin` nadpisz metodę `printName`


### Statyczne metody

#### Dodaj metodę statyczą `printHello` do definicji klasy `User`

```javascript
 User.printHello();
```