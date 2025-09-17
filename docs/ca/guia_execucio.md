### 📄 docs/guia_execucio.md

# Guia d'Execució - Projecte d'Animacions amb Manim

**🌐 Idioma / Language:** [Català](guia_execucio.md) | [English](../en/installation_guide.md)

Aquesta guia us ajudarà a configurar l'entorn i executar les animacions d'aquest Treball de Recerca en el vostre ordinador local.

## 📋 Prerequisits

Abans de començar, assegureu-vos de tenir instal·lats els següents programes:

### 1. Python (3.9 o superior)

- **Com comprovar-ho?** Obre una terminal i escriu:
  ```bash
  python --version
  # o
  python3 --version
  ```
- **Si no el tens**: Descarrega'l i instal·la'l des de [python.org](https://www.python.org/downloads/). **Important**: Durant la instal·lació, marca l'opció **"Add Python to PATH"**.

### 2. FFmpeg (Obligatori)

Manim utilitza FFmpeg per a renderitzar els vídeos.

- **Windows**:
  1.  Descarrega la darrera versió `full` de [gyan.dev](https://www.gyan.dev/ffmpeg/builds/).
  2.  Extreu la carpeta de l'arxiu ZIP (ex. a `C:\ffmpeg`).
  3.  **Afegeix FFmpeg al PATH** ([Guia visual](https://www.architectryan.com/2018/03/17/add-to-the-path-on-windows-10/)):
      - Cerca "Variables d'entorn" en el menú d'inici.
      - Cliqueu "Variables d'entorn..." → "Path" (d'usuari) → "Nou".
      - Afegiu la ruta a la carpeta `bin` dins de la carpeta FFmpeg (ex. `C:\ffmpeg\bin`).
- **macOS**:
  ```bash
  # Instal·la Homebrew si no el tens:
  /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
  # Instal·la FFmpeg:
  brew install ffmpeg
  ```
- **Linux (Debian/Ubuntu)**:
  ```bash
  sudo apt update && sudo apt install ffmpeg
  ```

### 3. LaTeX (MiKTeX) (Obligatori per a fórmules)

Necessari per renderitzar text i fórmules matemàtiques.

- **Windows**: Instal·la [MiKTeX](https://miktex.org/download). **Recomanat**: Triar l'opció "Install missing packages on the fly" durant la instal·lació.
- **macOS/Linux**: Instal·la [TeX Live](https://www.tug.org/texlive/).

## 🚀 Instal·lació i Execució

### Pas 1: Obtenir el codi font

Descarrega o clona aquest repositori en una carpeta del teu ordinador.

### Pas 2: Obri una terminal en la carpeta del projecte

Assegura't que la teva terminal està treballant dins del directori del projecte (on es troben els arxius `requirements.txt` i `README.md`).

### Pas 3: (Recomanat) Crear i activar un entorn virtual

Aïlla les dependències del projecte per evitar conflictes.

```bash
# Crear l'entorn virtual anomenat 'venv'
python -m venv venv

# Activar-lo
# A Windows:
venv\Scripts\activate
# A macOS/Linux:
source venv/bin/activate
```

**Nota**: Quan l'entorn virtual està activat, el prompt de la terminal mostrarà `(venv)` al principi.

### Pas 4: Instal·lar les dependències de Python

Amb l'entorn virtual activat, executa:

```bash
pip install -r requirements.txt
```

Això instal·larà la versió correcta de ManimCE (0.19.0) i totes les llibreries necessàries.

### Pas 5: Explorar i executar les animacions

Ja estàs tot preparat! Per veure quines animacions estan disponibles:

1.  **Explora els arxius Python** del projecte per veure les escenes disponibles.
2.  **Cerca classes que heretin de `Scene`** (o classes similars de Manim).
3.  **Executa una escena específica**:
    ```bash
    # Format: manim [opcions] arxiu.py ClasseDeLEscena
    manim -pqh arxiu.py ClasseDeLEscena
    ```

**Exemples de comandes**:

```bash
# Renderitza en alta qualitat i obre el vídeo
manim -pqh main.py IntroScene

# Renderitza en qualitat baixa (més ràpid) i reprodueix automàticament
manim -pql animations.py CircleToSquare

# Renderitza un GIF animat en lloc d'un vídeo
manim -pqh --format=gif scenes.py RotationExample

# Llista totes les escenes disponibles en un arxiu
manim --help scenes.py
```

Els vídeos renderitzats es guardaran a la carpeta `media/videos/` dins del teu projecte.

## 🆘 Solució de Problemes Comuns

- **Error: "FFmpeg not found"**:

  - Assegura't que el has instal·lat i que has **afegit la carpeta `bin` al PATH**. Tanca i reobri la terminal després de fer-ho.

- **Error: "LaTeX not found"**:

  - Assegura't que has instal·lat MiKTeX o TeX Live. En Windows, prova de reiniciar l'ordinador després de la instal·lació.

- **Error: "command not found: manim"**:

  - Assegura't que el teu entorn virtual està **activat** (`(venv)` ha d'aparèixer al prompt).
  - Assegura't que les dependències es van instal·lar correctament amb `pip install -r requirements.txt`.

- **No es veu el text matemàtic**:

  - Assegura't que LaTeX està instal·lat. MiKTeX pot demanar instal·lar paquets addicionals la primera vegada; permet-ho.

- **Error de versions de Python**:
  - Assegura't que tens Python 3.9 o superior. Si tens múltiples versions, utilitza `python3` en lloc de `python`.

## ℹ️ Informació Addicional

- **Documentació de ManimCE**: [https://docs.manim.community/](https://docs.manim.community/)
- **Repositori oficial**: [https://github.com/ManimCommunity/manim](https://github.com/ManimCommunity/manim)
- **Comunitat**: [Discord de Manim Community](https://manim.community/discord)

Si continues tenint problemes, pots:

1.  Verificar que tots els prerequisits estan instal·lats correctament
2.  Assegurar-te que l'entorn virtual està activat
3.  Consultar la documentació de ManimCE
4.  Obrir un "issue" en aquest repositori

**Que gaudeixis de les animacions! 🎬**

---

**🌐 Idioma / Language:** [Català](guia_execucio.md) | [English](../en/installation_guide.md)

```
