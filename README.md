# Visual Proofs in Secondary Mathematics / Demostracions Visuals per a les Matemàtiques de Secundària

[🇬🇧 English](#english) | [🇪🇸 Català](#català)

---

<a name="english"></a>
## 🇬🇧 English

A repository containing animations created with ManimCE for a high school research project (Treball de Recerca) titled **"Visual Mathematical Proofs for Secondary Education: An Accessible Approach with Digital Tools"**.

This project demonstrates, through **animations created with ManimCE**, how to construct essential mathematical formulas and theorems from **lower secondary education (ESO level)** step by step.

---

> **📚 Educational Level Note**  
> These animations focus on mathematical concepts taught in **ESO** (Educació Secundària Obligatòria), which corresponds to lower secondary education (typically ages 12–16) in the Spanish educational system. The content covers key concepts from algebra, geometry, and fundamental proofs appropriate for this level.

---

### 📂 Repository Structure

```
├── src/                          # Python source code (ManimCE scenes)
├── media/
│   ├── captures/                 # Representative animation frames
│   └── videos/                   # Rendered video files (optional)
├── docs/                         # Documentation (EN & CA)
└── requirements.txt              # Python dependencies
```

### 🚀 Installation & Usage

1. **Install Python 3.9+**
2. **Clone the repository**  
   ```bash
   git clone https://github.com/Jzhezheng08/TdR-demostracions-ESO
   ```
3. **Install dependencies**  
   ```bash
   pip install -r requirements.txt
   ```
4. **Run an animation**  
   ```bash
   manim -p -qh src/algebraic_identities.py
   ```

📖 *Detailed instructions: [Installation Guide](docs/en/installation_guide.md)*

---

### 🌐 Links

- **GitHub Repository**: [https://github.com/Jzhezheng08/TdR-demostracions-ESO](https://github.com/Jzhezheng08/TdR-demostracions-ESO)  
- **Animation Website**: *In progress*

---

<a name="català"></a>
## 🇪🇸 Català

Aquest repositori conté tot el codi font i els materials utilitzats en el **Treball de Recerca "Demostracions matemàtiques visuals de la ESO: un enfocament accessible amb eines digitals"**.

L'objectiu és mostrar, mitjançant **animacions creades amb ManimCE**, com es poden construir pas a pas les fórmules i teoremes matemàtics essencials de l'ESO.

---

### 📂 Estructura del repositori

```
├── src/                          # Codi font Python (escenes de ManimCE)
├── media/
│   ├── captures/                 # Captures de fotogrames representatius
│   └── videos/                   # Vídeos renderitzats (opcional)
├── docs/                         # Documentació (EN i CA)
└── requirements.txt              # Dependències de Python
```

### 🚀 Instal·lació i ús

1. **Instal·la Python 3.9+**
2. **Clona el repositori**  
   ```bash
   git clone https://github.com/Jzhezheng08/TdR-demostracions-ESO
   ```
3. **Instal·la les dependències**  
   ```bash
   pip install -r requirements.txt
   ```
4. **Executa una animació**  
   ```bash
   manim -p -qh src/identitats_algebraiques.py
   ```

📖 *Instruccions detallades: [Guia d'instal·lació](docs/ca/guia_execucio.md)*

---

### 🌐 Enllaços

- **Repositori GitHub**: [https://github.com/Jzhezheng08/TdR-demostracions-ESO](https://github.com/Jzhezheng08/TdR-demostracions-ESO)  
- **Lloc web amb animacions**: *En procés*

---

## 📚 Documentation

All documentation is available in both English and Catalan:

| Document Type | English | Català |
|---------------|---------|--------|
| Installation Guide | [English](docs/en/installation_guide.md) | [Català](docs/ca/guia_execucio.md) |
| Animation Explanations | [English](docs/en/animation_explanations.md) | [Català](docs/ca/explicacio_animacions.md) |

## 👥 Contributing

Contributions and translations are welcome! Feel free to open an issue or submit a pull request to make this project accessible to more students and educators worldwide.

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

> **Note**: This project was developed as part of a high school research project (Treball de Recerca) in Catalonia, Spain.
