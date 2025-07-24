# Arbore - Aplicație pentru Vizualizare și Operații pe Structuri de Date de Tip Arbore

## Contribuitor
- [COSTELINOO](https://github.com/COSTELINOO)

## Cerința problemei
Dezvoltarea unei aplicații desktop care permite vizualizarea, manipularea și operații pe structuri de date de tip arbore. Aplicația oferă funcționalități de autentificare a utilizatorilor, gestionare a sesiunilor, personalizare a interfeței și operații complexe pe arbori (creare, modificare, ștergere, sortare).

## Restricții și precizări
Proiectul este evaluat în funcție de complexitatea implementării, optimizarea algoritmilor, design-ul interfeței și experiența utilizatorului.

## Build and Run
Proiectul se poate compila și rula prin executarea scriptului `run.bat` (destinat pentru Windows).

## Videoclip de prezentare
[Link către videoclipul de prezentare a aplicației](https://drive.google.com/file/d/1gu82tia7zU_eD8UCEkG0hnON9PXzh7g-/view?usp=drive_link)

## Capturi de ecran
În această secțiune sunt prezentate câteva capturi de ecran reprezentative pentru aplicație:
- Ecranul de autentificare și înregistrare
- Meniul principal cu cele patru teme disponibile
- Vizualizarea arborelui și operațiile disponibile
- Exemple de creare, modificare și ștergere de noduri
- Demonstrarea funcționalității de sortare și căutare
<img width="1918" height="1013" alt="Screenshot 2024-07-12 124338" src="https://github.com/user-attachments/assets/5968e3fd-0462-4926-988c-1d55618bf136" />

<img width="1918" height="1015" alt="Screenshot 2024-07-12 124425" src="https://github.com/user-attachments/assets/36a8507f-5293-4a1b-8754-9743c0b06203" />

<img width="1918" height="1011" alt="Screenshot 2024-07-12 124446" src="https://github.com/user-attachments/assets/00dfdca2-76f0-46b6-8946-f38879fe60a3" />

<img width="1916" height="1017" alt="Screenshot 2024-07-12 124509" src="https://github.com/user-attachments/assets/0ad66900-8648-46cf-ab9b-42d73449c9c0" />

<img width="1918" height="1013" alt="Screenshot 2024-07-12 124527" src="https://github.com/user-attachments/assets/fb4b5b8c-3e72-4276-9e9c-ac9066e24931" />

<img width="1918" height="1017" alt="Screenshot 2024-07-12 124546" src="https://github.com/user-attachments/assets/1720cb0a-dd74-4ee2-8987-2828dee783f5" />

<img width="1918" height="1020" alt="Screenshot 2024-07-12 124635" src="https://github.com/user-attachments/assets/c216379e-e5c8-41d9-92b5-85e34ed076bf" />

<img width="1918" height="1012" alt="Screenshot 2024-07-12 124725" src="https://github.com/user-attachments/assets/c89c125b-2c0d-49e6-a2aa-334ac38e2a7b" />

<img width="1918" height="1012" alt="Screenshot 2024-07-12 124805" src="https://github.com/user-attachments/assets/5c8a0bfa-6389-4ea2-b973-89e624016597" />

<img width="1918" height="1015" alt="Screenshot 2024-07-12 124744" src="https://github.com/user-attachments/assets/37da07c0-789f-416c-8b5a-d079342ecc00" />


## Descriere generală
Aplicația "Arbore" este un instrument educațional și practic pentru lucrul cu structuri de date de tip arbore. Programul permite utilizatorilor să creeze, să vizualizeze și să manipuleze arbori, oferind o interfață grafică intuitivă pentru înțelegerea acestor structuri de date fundamentale în informatică.

## Funcționalități principale

### 1. Sistem de autentificare și înregistrare
- **Înregistrare utilizator**: Permite crearea unui cont nou cu username și parolă
- **Autentificare**: Sistem securizat de autentificare a utilizatorilor existenți
- **Persistența datelor**: Informațiile despre utilizatori sunt salvate într-un fișier text
- **Validare date**: Verificarea corectitudinii datelor introduse (caractere permise, lungime)

### 2. Personalizare interfață
- **Sistem de teme**: Aplicația oferă 4 teme diferite pentru personalizarea interfeței:
  - **Bear**: Temă în nuanțe de maro și auriu
  - **Aqua**: Temă în nuanțe de albastru și violet
  - **Emerald**: Temă în nuanțe de verde și portocaliu
  - **Space**: Temă în nuanțe de gri și negru
- **Persistența preferințelor**: Tema selectată este salvată și încărcată la următoarea autentificare

### 3. Vizualizare arbore
- **Reprezentare grafică**: Afișarea vizuală a arborelui cu noduri și legături
- **Deplasare (panning)**: Navigare în vizualizarea arborelui prin tragerea cu mouse-ul
- **Zoom in/out**: Controlul mărimii nodurilor și a textului pentru o vizualizare optimă
- **Revenire la rădăcină**: Recentrarea vizualizării la nodul rădăcină

### 4. Operații pe arbori
- **Crearea arborelui**: Definirea numărului maxim de fii pentru fiecare nod (între 1 și 1000)
- **Adăugare nod**: Inserarea unui nou nod în arbore cu specificarea unei chei (valori)
- **Modificare nod**: Schimbarea valorii unui nod existent
- **Ștergere nod/subarbore**: Eliminarea unui nod împreună cu toți descendenții săi
- **Sortare**: Ordonarea descendenților fiecărui nod după lungimea cheii și apoi alfabetic
- **Căutare**: Funcție de căutare a unui nod după valoarea sa

### 5. Navigare și interfață
- **Meniu principal**: Interfață pentru selectarea diferitelor funcționalități
- **Deconectare**: Posibilitatea de a ieși din cont și revenirea la ecranul de autentificare
- **Interfață intuitivă**: Design responsive și feedback vizual pentru acțiunile utilizatorului

## Structuri de date utilizate

### 1. Arbore digital (Trie)
- Utilizat pentru stocarea informațiilor despre utilizatori (username, parolă)
- Implementat prin structura `nod_arbore` care permite căutarea eficientă a utilizatorilor

### 2. Arbore general
- Structura principală a aplicației
- Implementat prin clasa `arbore` care permite un număr variabil de fii pentru fiecare nod
- Suportă diverse operații precum adăugare, ștergere, modificare, căutare și sortare

## Algoritmi implementați

### 1. Algoritm de desenare a arborelui
- Calculează pozițiile nodurilor pentru o vizualizare echilibrată
- Recalculează pozițiile la modificarea arborelui sau la operațiile de zoom

### 2. Algoritm de sortare (Merge Sort)
- Implementat pentru sortarea descendenților fiecărui nod
- Criteriile de sortare: nodurile nenule înaintea celor nule, lungimea cheii, ordinea alfabetică

### 3. Algoritmi de căutare
- Căutare în arbore digital (pentru autentificare)
- Căutare în arbore general (pentru găsirea nodurilor după valoare)

## Detalii de implementare

### Clase principale
- **fereastra**: Gestionează interfața grafică și interacțiunile utilizatorului
- **login**: Implementează funcționalitățile de autentificare și înregistrare
- **arbore**: Implementează structura de date și operațiile pe arbore
- **informatii_generale_arbore**: Conține informații globale despre starea arborelui

### Fișiere și persistența datelor
- Informațiile despre utilizatori sunt stocate în fișierul `utilizatori.txt`
- Formatul datelor: tema, username, parolă, indice_linie

## Tehnologii utilizate
- **Limbaj de programare**: C++
- **Bibliotecă grafică**: Raylib
- **Persistență date**: Fișiere text
