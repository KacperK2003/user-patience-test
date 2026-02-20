# User Patience Test

> Wersja polska | 🇬🇧 [See the English version](README.md)

## Autorzy
- Filip Gumiński ([@Fifikula](https://github.com/Fifikula))
- Kacper Kozłowski ([@KacperK2003](https://github.com/KacperK2003))
- Adam Rachuba ([@rachu033](https://github.com/rachu033))

**KAF Studio**

## Opis
Projekt ma na celu zbadanie, w jaki sposób różne typy animacji ładowania wpływają na postrzeganą cierpliwość użytkowników w środowisku aplikacji internetowej. Podsumowanie badania znajduje się w pliku KCK.pdf. 

## Technologie
- **Języki:** JavaScript, Python, HTML, CSS 
- **Framework:** Flask
- **Baza danych:** SQLite

## Uruchomienie projektu

### 1. Klonowanie repozytorium
```bash
git clone https://github.com/KacperK2003/user-patience-test.git
cd user-patience-test
```

### 2. Tworzenie i uruchomienie środowiska wirtualnego:
**Windows:**
```cmd
python -m venv .venv
.\.venv\Scripts\activate
```
Jeśli zwracany jest błąd ".venv\Scripts\Activate.ps1 cannot be loaded because running scripts is disabled on this system" użyj 
```cmd
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope Process
```

**Unix/macOS:**

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Instalowanie bibliotek:
```cmd
pip install -r .\requirements.txt
```


### 4. Stworzenie pliku .env:
Utwórz plik .env z tymi zmiennymi:
- DEBUG=TRUE or DEBUG=FALSE
- PORT={numer portu}

### 5. Inicjalizacja bazy danych SQLite:
```cmd
flask db init
flask db migrate
flask db upgrade
```


### 6. Uruchomienie projektu:
```cmd
python main.py
```

## Licencje

Kod źródłowy: Objęty licencją MIT License

Materiały badawcze (`KCK.pdf`): Objęty licencją [Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0)](https://creativecommons.org/licenses/by-nc/4.0/).

Prosimy o podanie autorów w przypadku wykorzystania lub cytowania wyników badania.


Zależności zewnętrzne:

| Biblioteka       | Licencja                                                     |
|------------------|--------------------------------------------------------------|
| Flask            | [BSD 3-Clause](https://opensource.org/licenses/BSD-3-Clause) |
| python-dotenv    | [BSD 3-Clause](https://opensource.org/licenses/BSD-3-Clause) |
| Flask-SQLAlchemy | [BSD 3-Clause](https://opensource.org/licenses/BSD-3-Clause) |
| Flask-Migrate    | [MIT](https://opensource.org/licenses/MIT)                   |
