[![pagepro_logo](https://miro.medium.com/fit/c/96/96/0*cVHxjMcinW8ale32.png)](https://daftcode.pl/)

# Praktyki Front-End (React) 2022

## Zadanie
Wykorzystując bibliotekę **ReactJS** stwórz aplikację służącą do przeglądania postaci z serialu *"Rick and Morty"*

Zadanie może zostać zrealizowane na różnym poziomie zaawansowania, który dobierzesz indywidualnie do posiadanej wiedzy oraz umiejętności.

Zadanie nie posiada projektu graficznego dlatego wszystkie widoki możesz zaprojektować wedle własnego uznania.   

## Poziom podstawowy

Podstawowa wersja aplikacji zakłada stworzenie listy postaci bazującej na statycznych danych dostępnych na samym dole.

### Wymagania:
- aplikacja składa się z dwóch podstawowych widoków:
  - **Lista postaci** - lista bazująca na udostępnionych, statycznych danych dostępna pod adresem `/characters`
  - **Szczegóły widok postaci** - dostępny pod adresem `/character/:id` np: `localhost:3000/character/5`
  
- Szczegółowy widok postaci będzie dostępny po kliknięciu w podlinkowany element na liście postaci np. nazwa postaci, avatar lub dowolny przycisk

*W przypadku tego zadania zostanie sprawdzona wiedza z zakresu podziału aplikacji na komponenty, przekazywania props-ów oraz konfiguracji routingu i przesyłania danych w jego obrębie*

## Poziom rozszerzony

Rozszerzona wersja aplikacji uwzględnia aplikację z wersji podstawowej wzbogaconą o dodatkowe funkcjonalnosci.

### Wymagania:
- Wszystkie funkcjonalności z `wersji podstawowej`
- Na liście postaci `/characters` przy każdym elemencie listy powinien znaleźć się przycisk umożliwiający dodanie postaci do listy ulubionych 
  - Po dodaniu postaci do ulubionych opcja ta zostaje zablokowana do momentu usunięcia postaci z listy ulubionych
  
- Dodatkowy widok **Lista ulubionych postaci** - dostępny pod adresem `/favourite-characters`.
  - Widok ten może być bliźniaczo podobny do listy postaci `/characters`
  - Na liście ulubionych postaci `/favourite-characters` przy każdym elemencie listy powinien znaleźć się przycisk umożliwiający usunięcie postaci z ulubionych

- W aplikacji powinna znaleźć się nawigacja umożliwiająca przechodzenie pomiędzy listą postaci `/characters`, a listą ulubionych postaci `/favourite-characters`

Funkcjonalność przechowywania i zarządzania listą ulubionych postaci może zostać zrealizowana w dowolny sposób (np. Context Api, Redux, State, Local Storage).
Dopuszczalne jest resetowanie listy ulubionych postaci po odświeżeniu aplikacji. 

*W przypadku tego zadania zostaną sprawdzone umiejętności z zakresu przechowywania danych oraz udostępniania ich pomiędzy dwoma komponentami znajdującymi się na tym samy poziomie, a także umiejętności związane z operacjami na tablicach.* 

## Poziom zaawansowany

Zaawansowana wersja aplikacji uwzględnia aplikację z wersji rozszerzonej wzbogaconą o dodatkowe funkcjonalnosci

### Wymagania:
- Wszystkie funkcjonalności z `wersji podstawowej` oraz `wersji rozszerzonej`
- integracja aplikacji z zewnętrznym api
  - Połącz swoją aplikację z zewnętnym api dostępnym na stronie [https://rickandmortyapi.com](https://rickandmortyapi.com)
  - **Dane listy postaci** - [https://rickandmortyapi.com/documentation/#get-all-characters](https://rickandmortyapi.com/documentation/#get-all-characters)
  - **Dane pojedynczej postaci** - [https://rickandmortyapi.com/documentation/#get-a-single-character](https://rickandmortyapi.com/documentation/#get-a-single-character)
  - **Dane wybranych postaci** - [https://rickandmortyapi.com/documentation/#get-multiple-characters](https://rickandmortyapi.com/documentation/#get-multiple-characters)

Dla osób korzystający z TypeScript lista interfejsów udostępnionego api [https://javascript.rickandmortyapi.com/modules/interfaces.html](https://javascript.rickandmortyapi.com/modules/interfaces.html)

*W przypadku tego zadania zostaną sprawdzone umiejętności z zakresu integracji, z REST API, oraz pracy z dokumentacją*

## Podsumowanie
Stworzone zadanie stara się odzwierciedlić podstawowe wyzwania, które stawiane są przed programistami Front-End w ich codziennej pracy.

Jeśli nie jesteś w stanie rozwiązać zadania z wyższego poziomu zaawansowania, nic nie szkodzi. 
Wyślij nam to co udało Ci się osiągnąć i ciesz się z wiedzy opanowanej w trakcie realizacji.

Jeśli natomiast przedstawione wymagania to dla Ciebie *"bułka z masłem"* pomyśl o rozbudowaniu swojej aplikacji o następujące funkcjonalności:
- wyszukiwarka
- filtry
- paginacja
- loadery przy pobieraniu danych
- dostosowanie do RWD *(Responsive Web Design)*

Lub zaproponuj coś od siebie! Pomysłowość jest zawsze w cenie!

## Na co będziemy zwracać uwagę
- Dobre praktyki oraz czystość kodu,
- Odpowiedni podział logiki na komponenty
- Zasadność użytych techologii oraz bibliotek

## Mile widziane
- TypeScript

## Przesłanie gotowego rozwiązania
- Najlepszym rozwiązaniem będzie stworzenie publicznego repozytorium oraz przesłanie nam do niego liknu.
- Aplikacja nie musi być hostowana lecz jeśli chcesz to zrobić, to nie mamy nic przeciwko.

## Dane do zadania (poziom podstawowy oraz rozszerzony)

```json
[
  {
  "id": 1,
  "name": "Rick Sanchez",
  "status": "Alive",
  "species": "Human",
  "type": "",
  "gender": "Male",
  "origin": { "name": "Earth (C-137)" },
  "location": { "name": "Citadel of Ricks" },
  "image": "https://rickandmortyapi.com/api/character/avatar/1.jpeg",
  "created": "2017-11-04T18:48:46.250Z"
  },
  {
  "id": 2,
  "name": "Morty Smith",
  "status": "Alive",
  "species": "Human",
  "type": "",
  "gender": "Male",
  "origin": { "name": "unknown" },
  "location": { "name": "Citadel of Ricks" },
  "image": "https://rickandmortyapi.com/api/character/avatar/2.jpeg",
  "created": "2017-11-04T18:50:21.651Z"
  },
  {
  "id": 3,
  "name": "Summer Smith",
  "status": "Alive",
  "species": "Human",
  "type": "",
  "gender": "Female",
  "origin": { "name": "Earth (Replacement Dimension)"},
  "location": { "name": "Earth (Replacement Dimension)"},
  "image": "https://rickandmortyapi.com/api/character/avatar/3.jpeg",
  "created": "2017-11-04T19:09:56.428Z"
  },
  {
  "id": 4,
  "name": "Beth Smith",
  "status": "Alive",
  "species": "Human",
  "type": "",
  "gender": "Female",
  "origin": { "name": "Earth (Replacement Dimension)" },
  "location": { "name": "Earth (Replacement Dimension)" },
  "image": "https://rickandmortyapi.com/api/character/avatar/4.jpeg",
  "created": "2017-11-04T19:22:43.665Z"
  },
  {
  "id": 5,
  "name": "Jerry Smith",
  "status": "Alive",
  "species": "Human",
  "type": "",
  "gender": "Male",
  "origin": { "name": "Earth (Replacement Dimension)"},
  "location": { "name": "Earth (Replacement Dimension)"},
  "image": "https://rickandmortyapi.com/api/character/avatar/5.jpeg",
  "created": "2017-11-04T19:26:56.301Z"
  },
  {
  "id": 6,
  "name": "Abadango Cluster Princess",
  "status": "Alive",
  "species": "Alien",
  "type": "",
  "gender": "Female",
  "origin": { "name": "Abadango" },
  "location": { "name": "Abadango" },
  "image": "https://rickandmortyapi.com/api/character/avatar/6.jpeg",
  "created": "2017-11-04T19:50:28.250Z"
  },
  {
  "id": 7,
  "name": "Abradolf Lincler",
  "status": "unknown",
  "species": "Human",
  "type": "Genetic experiment",
  "gender": "Male",
  "origin": { "name": "Earth (Replacement Dimension)" },
  "location": { "name": "Testicle Monster Dimension" },
  "image": "https://rickandmortyapi.com/api/character/avatar/7.jpeg",
  "created": "2017-11-04T19:59:20.523Z"
  },
  {
  "id": 8,
  "name": "Adjudicator Rick",
  "status": "Dead",
  "species": "Human",
  "type": "",
  "gender": "Male",
  "origin": { "name": "unknown" },
  "location": { "name": "Citadel of Ricks" },
  "image": "https://rickandmortyapi.com/api/character/avatar/8.jpeg",
  "created": "2017-11-04T20:03:34.737Z"
  },
  {
  "id": 9,
  "name": "Agency Director",
  "status": "Dead",
  "species": "Human",
  "type": "",
  "gender": "Male",
  "origin": { "name": "Earth (Replacement Dimension)" },
  "location": { "name": "Earth (Replacement Dimension)" },
  "image": "https://rickandmortyapi.com/api/character/avatar/9.jpeg",
  "created": "2017-11-04T20:06:54.976Z"
  },
  {
  "id": 10,
  "name": "Alan Rails",
  "status": "Dead",
  "species": "Human",
  "type": "Superhuman (Ghost trains summoner)",
  "gender": "Male",
  "origin": { "name": "unknown" },
  "location": { "name": "Worldender's lair" },
  "image": "https://rickandmortyapi.com/api/character/avatar/10.jpeg",
  "created": "2017-11-04T20:19:09.017Z"
  },
  {
  "id": 11,
  "name": "Albert Einstein",
  "status": "Dead",
  "species": "Human",
  "type": "",
  "gender": "Male",
  "origin": { "name": "Earth (C-137)" },
  "location": { "name": "Earth (Replacement Dimension)" },
  "image": "https://rickandmortyapi.com/api/character/avatar/11.jpeg",
  "created": "2017-11-04T20:20:20.965Z"
  },
  {
  "id": 12,
  "name": "Alexander",
  "status": "Dead",
  "species": "Human",
  "type": "",
  "gender": "Male",
  "origin": { "name": "Earth (C-137)" },
  "location": { "name": "Anatomy Park" },
  "image": "https://rickandmortyapi.com/api/character/avatar/12.jpeg",
  "created": "2017-11-04T20:32:33.144Z"
  },
  {
  "id": 13,
  "name": "Alien Googah",
  "status": "unknown",
  "species": "Alien",
  "type": "",
  "gender": "unknown",
  "origin": { "name": "unknown" },
  "location": { "name": "Earth (Replacement Dimension)" },
  "image": "https://rickandmortyapi.com/api/character/avatar/13.jpeg",
  "created": "2017-11-04T20:33:30.779Z"
  },
  {
  "id": 14,
  "name": "Alien Morty",
  "status": "unknown",
  "species": "Alien",
  "type": "",
  "gender": "Male",
  "origin": { "name": "unknown" },
  "location": { "name": "Citadel of Ricks" },
  "image": "https://rickandmortyapi.com/api/character/avatar/14.jpeg",
  "created": "2017-11-04T20:51:31.373Z"
  },
  {
  "id": 15,
  "name": "Alien Rick",
  "status": "unknown",
  "species": "Alien",
  "type": "",
  "gender": "Male",
  "origin": { "name": "unknown" },
  "location": { "name": "Citadel of Ricks" },
  "image": "https://rickandmortyapi.com/api/character/avatar/15.jpeg",
  "created": "2017-11-04T20:56:13.215Z"
  },
  {
  "id": 16,
  "name": "Amish Cyborg",
  "status": "Dead",
  "species": "Alien",
  "type": "Parasite",
  "gender": "Male",
  "origin": { "name": "unknown" },
  "location": { "name": "Earth (Replacement Dimension)" },
  "image": "https://rickandmortyapi.com/api/character/avatar/16.jpeg",
  "created": "2017-11-04T21:12:45.235Z"
  },
  {
  "id": 17,
  "name": "Annie",
  "status": "Alive",
  "species": "Human",
  "type": "",
  "gender": "Female",
  "origin": { "name": "Earth (C-137)" },
  "location": { "name": "Anatomy Park" },
  "image": "https://rickandmortyapi.com/api/character/avatar/17.jpeg",
  "created": "2017-11-04T22:21:24.481Z"
  },
  {
  "id": 18,
  "name": "Antenna Morty",
  "status": "Alive",
  "species": "Human",
  "type": "Human with antennae",
  "gender": "Male",
  "origin": { "name": "unknown" },
  "location": { "name": "Citadel of Ricks" },
  "image": "https://rickandmortyapi.com/api/character/avatar/18.jpeg",
  "created": "2017-11-04T22:25:29.008Z"
  },
  {
  "id": 19,
  "name": "Antenna Rick",
  "status": "unknown",
  "species": "Human",
  "type": "Human with antennae",
  "gender": "Male",
  "origin": { "name": "unknown" },
  "location": { "name": "unknown" },
  "image": "https://rickandmortyapi.com/api/character/avatar/19.jpeg",
  "created": "2017-11-04T22:28:13.756Z"
  },
  {
  "id": 20,
  "name": "Ants in my Eyes Johnson",
  "status": "unknown",
  "species": "Human",
  "type": "Human with ants in his eyes",
  "gender": "Male",
  "origin": { "name": "unknown" },
  "location": { "name": "Interdimensional Cable" },
  "image": "https://rickandmortyapi.com/api/character/avatar/20.jpeg",
  "created": "2017-11-04T22:34:53.659Z"
  }
]
```
