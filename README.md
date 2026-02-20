# User Patience Test

> English version | 🇵🇱 [Zobacz wersję po polsku](README.pl.md)

## Authors
- Filip Gumiński ([@Fifikula](https://github.com/Fifikula))
- Kacper Kozłowski ([@KacperK2003](https://github.com/KacperK2003))
- Adam Rachuba ([@rachu033](https://github.com/rachu033))

**KAF Studio**

## Description
The project aims to examine how different types of loading animations affect users' perceived patience in a web application environment. The summary of the study is in the KCK.pdf file. 

## Technologies
- **Languages:** JavaScript, Python, HTML, CSS 
- **Framework:** Flask
- **Database:** SQLite

## Running the project

### 1. Cloning the repository
```bash
git clone https://github.com/KacperK2003/user-patience-test.git
cd user-patience-test
```

### 2. Creating and running the virtual environment:
**Windows:**
```cmd
python -m venv .venv
.\.venv\Scripts\activate
```
If there is the error ".venv\Scripts\Activate.ps1 cannot be loaded because running scripts is disabled on this system" use 
```cmd
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope Process
```

**Unix/macOS:**
```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Installing the libraries:
```cmd
pip install -r .\requirements.txt
```


### 4. Creating the .env file:
Create the .env file with those variables:
- DEBUG=TRUE or DEBUG=FALSE
- PORT={port number}

### 5. Initializing the SQLite database:
```cmd
flask db init
flask db migrate
flask db upgrade
```


### 6. Running the project:
```cmd
python main.py
```

## Licenses

Source code: Licensed under the MIT License
The research materials (`KCK.pdf`): Licensed under the [Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0)](https://creativecommons.org/licenses/by-nc/4.0/).

Please credit the original authors if you use or reference any part of the research.

External dependencies:

| Library          | License                                                      |
|------------------|--------------------------------------------------------------|
| Flask            | [BSD 3-Clause](https://opensource.org/licenses/BSD-3-Clause) |
| python-dotenv    | [BSD 3-Clause](https://opensource.org/licenses/BSD-3-Clause) |
| Flask-SQLAlchemy | [BSD 3-Clause](https://opensource.org/licenses/BSD-3-Clause) |
| Flask-Migrate    | [MIT](https://opensource.org/licenses/MIT)                   |
